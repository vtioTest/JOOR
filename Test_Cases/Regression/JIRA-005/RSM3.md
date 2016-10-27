##Test: Regression JIRA-005

###Application: JOOR User Home page

###Functionality: Send New Message

**Pre-requisites**:

 * Active user set up (qatest1/qatest1)

 * Create valid message recipients ( joor, JOOR Florida, JOOR Regress)

 * Testing environment (staging.joordev.com)

**Test Case RSM3**: Positive scenario with message sent to all connections

*Need more requirements for this functionality, the default values and valid options to complete the TC*

**Steps**:

1. Clear browser cache
2. Load URL (staging.joordev.com), verify correct domain is loaded and verify UI against the mockup
3. Login using valid user credentials
4. Verify correct user page is displayed (user name is displayed in the upper right corner) and verify UI against the mockup
5. Select &quot;Messages&quot; on the page menu
6. From drop down menu, select &quot;Send a Message&quot;
7. Verify correct dialog box is displayed, &quot;Compose a Message&quot;
8. Select radio button for all recipients &quot;SEND TO ALL MY CONNECTIONS&quot;
9. Verify that the input box &quot;RECIPIENT(S)&quot;  is not displayed on the form
10. Enter text in SUBJECT input box
11. Enter text in MESSAGE input box
12. \*Optional (need more info on the requirements): Attach a test file and verify it is attached (the file name is displayed next to the attachment action button)
13. Select button &quot;SEND&quot; to send the message
14. Verify that the INBOX page is displayed upon successful message submission
15. Verify the sent message is displayed in the SENT tab with correct recipients, subject and date (current set up seems to have &quot;joor&quot; as the default recipient when selecting all connections)
16. Verify the sent message is recorded in db (depends on your procedures)
17. Logout
