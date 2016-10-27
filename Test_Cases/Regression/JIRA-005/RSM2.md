##Test: Regression JIRA-005

###Application: JOOR User Home page

###Functionality: Send New Message

**Pre-requisites**:

 * Active user set up (qatest1/qatest1)

 * Create valid message recipients ( joor, JOOR Florida, JOOR Regress)

 * Testing environment (staging.joordev.com)

**Test Case RSM2**: Positive scenario, selecting multiple recipients

*Need requirements on the behavior of the Recipient(s) drop down box to be able to provide verification steps for it*

**Steps**:

1. Clear Browser cache
2. Load URL, verify correct domain is loaded, verify page UI against mockup
3. Login using valid user credentials
4. Verify correct user page is displayed (user name is displayed in the upper right corner) and verify UI against the mockup
5. Select &quot;Messages&quot; on the page menu
6. From drop down menu, select &quot;Send a Message&quot;
7. Verify correct dialog box is displayed, &quot;Compose a Message&quot;
8. Select radio button &quot;SEND TO ALL MY CONNECTIONS&quot;
9. Verify that the input box &quot;RECIPIENT(S)&quot;  is not displayed
10. Enter the recipient&#39;s address, e.g.: &quot;joor&quot;
11. Enter the next recipient&#39;s address, e.g.: &quot;JOOR Regress&quot;
12. Verify all of the selected recipient are displayed in bold text above &quot;RECIPIENT(S)&quot; input box
13. Verify that each of the selected recipients&#39; names has action button to remove it to the left of the name displayed ( &quot;x&quot;)
14. Remove one of the names and verify it is no longer listed above &quot;RECIPIENT(S)&quot; input box
15. Enter text in SUBJECT input box
16. Enter text in MESSAGE input box
17. \*Optional(Need more info on the requirements): Attach a test file and verify it is attached (the file name is displayed next to the attachment action button).
18. Select button &quot;SEND&quot; to send the message
19. Verify that the INBOX page is displayed upon successful message submission
20. Verify the sent message is displayed in the SENT tab with correct attributes (recipient, subject, date)
21. Verify the sent message is recorded in db (depends on your procedures)
22. Logout
