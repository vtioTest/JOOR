##Test: Regression JIRA-005

###Application: JOOR User Home page

###Functionality: Send New Message

**Pre-requisites**:

 * Active user set up (qatest1/qatest1)

 * Create valid message recipients ( joor, JOOR Florida, JOOR Regress)

 * Testing environment (staging.joordev.com)

**Test Case RSM1**: Positive scenario with selecting a single message recipient

*Need requirements on the behavior of the Recipient(s) drop down box to be able to provide verification steps for it*

**Steps**:

1. Clear Browser cache
2. Load URL, verify correct domain is loaded, verify page UI against mockup
3. Login using valid user credentials
4. Verify correct user page is displayed (user name is displayed in the upper right corner) and verify UI against the mockup
5. Select &quot;Messages&quot; on the page menu
6. From drop down menu, select &quot;Send a Message&quot;
7. Verify correct dialog box is displayed, &quot;Compose a Message&quot;
8. Select radio button &quot;SELECT CONNECTIONS&quot;
9. Verify that the input box &quot;RECIPIENT(S)&quot;  is displayed now
10. Enter the recipient&#39;s address, e.g.: &quot;joor&quot;
11. Verify the selected recipient is displayed in bold text above &quot;RECIPIENT(S)&quot; input box
12. Verify the selected recipient&#39;s name is displayed to the right of the action button &quot;x&quot; (allows to remove the recipient)
13. Enter text in SUBJECT input box
14. Enter text in MESSAGE input box
15. \*Optional (need info on the requirements): Attach a test file and verify it is attached (the file name is displayed next to the attachment action button)
16. Select button &quot;SEND&quot; to send the message
17. Verify that the INBOX page is displayed upon successful message submission
18. Select SENT tab and verify the sent message is displayed in the SENT tab with correct attributes (recipient, subject, date)
19. Verify the sent message is recorded in db (depends on your procedures)?
20. Logout
