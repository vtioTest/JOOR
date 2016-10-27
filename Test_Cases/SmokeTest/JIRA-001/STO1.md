##Test: Smoke Test JIRA-001

###Application: JOOR User Home page

###Functionality: Create a Pending Order

**Pre-requisites**:

 * Active user set up (qatest1/qatest1)

 * Create valid message recipients ( joor, JOOR Florida, JOOR Regress)

 * Testing environment (staging.joordev.com)

*Ideally smoke test would be automated with a tool like Selenium*

*Need more info on reqs for selecting valid order options*



**STO1**: Smoke test for Pending Order

**Steps**:

1. Clear Browser cache
2. Load home page URL, verify correct domain is loaded, verify page UI against mockup
3. Login using valid user credentials
4. Select &quot;Orders&quot; on page menu
5. Select &quot;Start Order&quot; from drop down menu
6. Verify correct form is displayed
7. Select &quot;Web Order&quot; from the Start Order dialog box
8. Enter valid parameters into input boxes (\*need requirements on valid options), usually the first or last option from drop down list
9. Select &quot;Start Order&quot; button
10. Select first or last (to avoid having too few items listed) from the items listed and select &quot;Buy&quot;
11. Choose quantity for each size desired (order must meet 1000USD min requirement) and enter color comment &quot;test color&quot;on the Order Info Form displayed
12. Select &quot;Add &amp; View Cart&quot; button
13. Verify Cart page is displayed with correct item and size quantities
14. Select Checkout
15. Select required values: Shipping method and Payment method (first available option from the dropdown)
16. Select &quot;Pending&quot; button
17. On &quot;Confirm Pending Order&quot; dialog box, enter the Subject text and Message text if desired (\*need info on requirements) or just select &quot;Submit&quot; button
18. Verify &quot;Review Order&quot; page is displayed with correct order info
19. Logout
