##Test: Regression JIRA-005

###Application: JOOR User Home page

###Functionality: Send New Message

**Pre-requisites**:

 * Active user set up (qatest1/qatest1)

 * Create valid message recipients ( joor, JOOR Florida, JOOR Regress)

 * Testing environment (staging.joordev.com)

**Test Case RSM4**: Positive Scenario with missing required data

*Need more information on requirements for the error dialog box as there is inconsistency with the form depending on browser (&quot;OK&quot; to close out dialog in Chrome with unformatted dialog box header and &quot;Close&quot; button to close out the dialog box in Safari. Also, in Chrome  the dialog box persists on the user screen even if switch tabs, and error dialog box is not appearing in FF. Requirements for the error dialog box are needed to write an efficient automated test case.)*

**Steps**:

1. Clear browser cache
2. Load URL (staging.joordev.com), verify correct domain is loaded and verify UI against the mockup
3. Login using valid user credentials
4. Verify correct user page is displayed (user name is displayed in the upper right corner)
5. Select &quot;Messages&quot; on the page menu
6. From drop down menu, select &quot;Send a Message&quot;
7. Verify correct dialog box is displayed, &quot;Compose a Message&quot;
8. Click &quot;SEND&quot;
9. Verify pop-up error message is displayed &quot;Your message could not be sent. Please ensure the message subject and body are not empty.&quot;
10. Click &quot;OK&quot; to close the pop-up
11. Enter recipient address in the RECIPIENT input box and click &quot;SEND&quot;
12. Verify pop-up error message is displayed &quot;Your message could not be sent. Please ensure the message subject and body are not empty.&quot;
13. Click &quot;OK&quot; to close the pop-up
14. Enter text in SUBJECT input box and click &quot;SEND&quot;
15. Verify pop-up error message is displayed &quot;Your message could not be sent. Please ensure the message subject and body are not empty.&quot;
16. Click &quot;OK&quot; to close the pop-up
17. Enter text in MESSAGE input box and click &quot;SEND&quot;
18. Verify pop-up error message is displayed &quot;Your message could not be sent.  Please check your recipients list and try again.&quot;
19. Click &quot;OK&quot; to close the pop-up
20. Select radio button to select recipient(s)
21. Click &quot;SEND&quot;
22. Verify pop-up error message is displayed &quot;Your message could not be sent.  Please check your recipients list and try again.&quot;
23. Click &quot;OK to close the pop-up
24. Enter recipient address in the RECIPIENT(S) input box
25. Click &quot;SEND&quot;
26. Verify message is submitted successfully, no error is displayed
27. Logout
