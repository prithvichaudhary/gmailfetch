# gmailfetch

If you are ever curious to know how we can fetch Gmail e-mails using Python then this article is for you.
As we know Python is a multi-utility language which can be used to do a wide range of tasks. Fetching Gmail emails though is a tedious task but with Python, many things can be done if you are well versed with its usage. Gmail provides IMAP access to clients who want to access Gmail without manually logging in the browser.

In setting page, enable this before running script. 

![image](https://github.com/prithvichaudhary/gmailfetch/assets/104778560/ebb271ae-eaa5-473b-87b0-165ca857899a)



Implementation: 
The libraries used in this implementation includes imaplib, email. You have to manually go and make IMAP access enabled by going into your Gmail account settings. After this only you could access your Gmail account without logging in browser. 

Three functions are defined in the implementation which is used to get email body, search for emails from a particular user and get all emails under a label.
For showing results I have sent email to my id from my another Gmail account. Now I will be fetching emails from my Gmail account which is received from my another Gmail account.
The process begins from making Gmail connection with the help of imaplib library and proving our Gmail login credentials to it.
After logging we are selecting emails under the label: Inbox which is a default labeled section for all users. However, you can create your own labels also.
Then we are calling get emails function and provide it the parameter from search function result i.e “from user”
In get emails function we are putting all emails in an array named “msgs”
Now print to see the msgs array
Now we can easily iterate over this array. We are iterating it in the order the emails arrived. Then we are searching for the index from where our content begins. This indexing part will be different for different emails/users and the user can manually change the indexes to print only that part which they require.
We have our results printed out.
