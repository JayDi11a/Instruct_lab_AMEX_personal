Title: Actimize Alerts \- Amex Checking Fraud
Overview:
How to process adjudicate ACH, wire, or check alerts in Actimize.
Key details
An Admin can stop transactions that are claimed as fraud on behalf of other users; however, only
a Primary can clear concerns stemming from an Actimize alert.
", "
Review alerts
Note: Retail Party Activity shows ACH and wire transactions. Deposit Account Activity shows
check transactions.
Step 1
1\. Access Actimize.
2\. Go to Workbench \> Work Items.
3\. Select the appropriate Work Items for the queue currently assigned by your Leadership
team.
Fraud Queue Description
Account Take Alerts where there is a concern that the account has been taken over by a
Over (ATO) third\-party using stolen credentials.
Alerts where there is a concern that a customer is intending to defraud or
First Party
intentionally cause loss to Amex. They may use their own identity or a
Fraud
fictitious identity.
Fraud Alerts where there is a concern that a person has opened an account using
Application stolen information (name, address, Social Security Number (SSN), Employer
(FRAP) Identification Number (EIN), etc.) to commit fraud.
Alerts where there is a concern that a customer has initiated a large
High Dollar
transaction.
Alerts where there is a concern where a customer has initiated a transaction
High Risk
that poses a greater exposure for fraud or loss.

Known Fraud
Alerts where there is a concern initiated by an identified fraud ring.
Rings
Same Day ACH A customer initiates an expedited transaction request.
Wires \-
A customer initiates an outgoing wire transaction request.
Checking
Note: Only one Work Items queue can be accessed at a time.
Step 2
1\. Organize the results by Item Date and begin the process with the oldest dated item.
2\. Click on the Item ID.
3\. What is the Step of the alert?
1\. Click Next Steps from the drop\-down.
2\. Select In Process.
Ready
Go to the next step.
click Next Steps \> Attempting Contact Customer Day
Ready to Contact Customer Day 2 \> OK.
2
Go to the next step.
Step 3
1\. Access the Transactions At Risk section.
2\. Click the check box next to each Item ID. (If more than 3 must select Show all)
3\. Click Actions.
4\. Select Change Step and click Execute.
5\. Select In Process as Next Step.
6\. Click Ok.
Step 4
1\. Select the applicable Item IDs, one at a time. This will take you to Retail Monetary
ActivityACH Same Day or Retail Monetary Activity or Deposit Activity screen.
2\. Joint Rewards Checking accounts: You can identify which Customer initiated the
transaction through Transaction Events where the Customerâ€™s unique Customer ID
(5201\.7000XXX) will display in the User ID field.
3\. Review and make note of Detection Policy Rules that triggered to use in your review.
4\. Access the account within MBP BOUI.
5\. Investigate for suspected fraud.

For Retail Monetary Activity ACH Same Day or Retail Monetary Activity:
• Review and make note of Analytics Issues, Party Details, Counter Party/Payee Details
Session Information, and Historical Party Activity in Actimize.
• Compare Customer identity using GSP and/or Lexis Nexis. For example, Customer name,
SSN, address, dob, and phone.
For Deposit Activity:
• Review check in ImageOne by dollar amount and date of deposit.
• Review Analytics Issues, Party Details, Session Information, and Historical Party
Activity in Actimize.
• Confirm Customer identity using GSP and/or Lexis Nexis. For example, Customer name,
SSN, address, DOB, phone.
Step 5
Has the Customer had 2 or more ACH and check returns in the last 6 months?
Has first party fraud been ruled out?
Yes
• Yes: Go to the next step.
• No: Go to First Party Fraud â€“ Identify and Handle.
No Go to the next step.
Step 6
Perform a Fraud Risk Review and take all applicable actions per procedure, then go to the next
step.
Step 7
Was the alert generated due to Fraud Monitoring Status (M\-Stat)?
1\. Review MBP BOUI notes.
2\. Has the High Focus Customer fraud monitoring been present for 30 or more calendar
days?
YesNote: MBP BOUI notes may indicate a previous extension of the High Focus Customer
fraud monitoring.
• Yes: Go to the next step.
• No: Go to step 9\.
No Go to step 9\.

Step 8
1\. Review closure status of previous Actimize alerts.
2\. Review transaction history in MBP BOUI.
3\. Are there any negative transaction actions in the last 30 days? For example, returns or
rejected Actimize alerts.
M\-stat will remain for another 30 days.
Yes
Go to the next step.
Remove from High Focus Customer fraud monitoring:
• In Actimize, go to Settings \> Platform Lists.
No • Select High Focus Customer.
• Locate and check mark the Party Key (Customer ID) needing to be removed.
• Select Delete.
Go to the next step.
Step 9
Per your fraud risk and/or first party fraud review in above steps, are there fraud concerns that
warrant stopping the transaction?
YesGo to step 17 to close the alert as Closed Fraud or Suspected Fraud.
No Go to the next step.
Step 10
Is the transaction an outgoing wire of $5,000 or more?
YesGo to the next step.
No Go to step 17 to close the alert as Closed Non\-Fraud.
Step 11
Perform an EWS name verification of the recipient of funds.
Is there an N result on both First Name and Last Name or Business Name or displays No Known
Information?
YesGo to Step 14\.
No Go to the next step.
Step 12
I s the transaction on a Business checking account?

Is the transaction an outgoing wire of $50,000 or more?
Yes
YesGo to step 14\.
No Go to step 17 to close the alert as Closed Non\-Fraud.
No Go to the next step.
Step 13
Is the transaction an outgoing wire of $15,000 of more?
YesGo to the next step.
No Go to step 17 to close the alert as Closed Non\-Fraud.
Step 14
Contact the Customer who initiated the wire at a BEPN to confirm wire transaction details.
Refer to Best Established Phone Number.
The Customer is
Go to step 16\.
available.
Leave this message: This message is for (Customerâ€™s full name). This is
(your name) calling from American Express National Bank. Please return
our call at 1\-855\-497\-1040\. And provide reference number (insert case
The Customer is reference number). Our hours of operation are 7:00 am to 7:00 pm MT
unavailable. Monday through Friday. Thank you, we look forward to speaking with
you.
Go to the next step.
No BEPN is
available for the Go to the next step.
Customer.
Step 15
1\. Send a General Fraud Servicing Please Contact Us communication via Control Tower.
2\. Perform the following for both child and parent case alerts:
1\. Click Next Steps \> Contact Attempted Day 1 (or Day 2\).
2\. Select Contact customer attempted at \[month/day/year] \[hour:minute AM/PM
timezone]. No answer. from the Add Note drop\-down.
3\. Add notes in MBP BOUI, including the following template (use N/A where not
applicable):
◦ Did you contact the customer at a BEPN (include Lexis Nexis report ID)?
◦ If applicable, was the customer advised with verbal or email notice that payment
was rejected or cancelled?
◦ If applicable, was the wire cancelled, upon learning the account holder (wire
submitter) was deceased or incompetent?
◦ If the recipientâ€™s name and account number did not match, was the wire
cancelled?
Process complete.

Step 16
Did the Customer initiate the outgoing wire transaction?
1\. Ask the Customer to confirm the wire details (amount and recipient).
◦ Cancel the request if the Customer needs to change the wire amount or
recipient (follow Customer Cancellation Requests, if appropriate). They must
submit a new request with the new details.
◦ Using the following template, note the account in MBP BOUI (use N/A where
not applicable):
▪ Did you contact the customer at a BEPN, (include Lexis Nexis report
Yes ID)?.
▪ If applicable, was the customer advised with verbal or email notice
that payment was rejected or cancelled?
▪ If applicable, was the wire cancelled, upon learning the account
holder (wire submitter) was deceased or incompetent?
▪ If the recipientâ€™s name and account number did not match, was
the wire cancelled?
2\. Go to the next step to close the alert as Closed Non\-Fraud.
1\. Handle the account as Account Taken Over (ATO).
2\. Using the following template, note the account in MBP BOUI (use N/A where not
applicable):
1\. Did you contact the customer at a BEPN, (include Lexis Nexis report ID)?.
2\. If applicable, was the customer advised with verbal or email notice that
No payment was rejected or cancelled?
3\. If applicable, was the wire cancelled, upon learning the account holder
(wire submitter) was deceased or incompetent?
4\. If the recipientâ€™s name and account number did not match, was the wire
cancelled?
3\. Go to the next step to close the alert as Closed Fraud.
Step 17
1\. Click Next Steps from the drop\-down and select the applicable closure action. See Alert
Closure Matrix.
2\. Select the applicable Reason. See Alert Closure Matrix below.
3\. Add Notes, including any Lexis Nexis report ID.
4\. Click OK.
5\. Click Navigate Back To arrow.
Step 18
Create an nGage case to capture any confirmed fraud activity, if applicable. Refer to nGage
Fraud Dispute Claim.
Step 19
1\. Repeat steps for all Transactions At Risk items until all are closed.
◦ Note: For Retail Monetary Activity ACH Same Day alerts, work all same day
ACH items before working party level alerts that are non\-same day ACH.
2\. On the Retail Party Activity or Deposit Account Activity screen, click Next Steps from
the drop\-down.

3\. Select the appropriate action from the Next Steps drop\-down. See Alert Closure Matrix
below.
◦ Note: If at least one Transaction At Risk item is closed fraud, then close the Retail
Party Activity alert as Fraud.
4\. Select the applicable Reason. See Alert Closure Matrix below.
5\. Add Notes, including any Lexis Nexis report ID.
6\. Click OK.
7\. Leave notes in MBP BOUI on the Customer/organization level, indicating the outcome of
your review and any actions taken.
8\. Click Navigate Back To arrow.
Step 20
Prior to day end cutoff time, perform the following steps:
• Standard ACH alerts received prior to 7:00 pm ET must be reviewed by 8:45 pm ET same
day.
• Wire alerts time stamped by 4:00 pm ET must be reviewed by 6:00 pm ET same day.
• Expedited/same day ACH alerts received prior to 2:45 pm ET must be reviewed by 4:15
pm ET same day.
1\. Access Actimize.
2\. Go to Workbench \> Work Items.
3\. Select Retail Monetary Activity ACH Same Day or Retail Monetary Activity.
4\. Determine if any alerts are still open.
YesGo to Step 4\.
No Process complete.
", "
Customer Call \- Alert Handling
Step 1
Was the Customer properly authenticated?
Note: No further authentication is required if an outbound call was placed to the Customer at a
verified BEPN.
YesGo to the next step.
Authenticate the Customer.
No
Go to the next step.
Step 2
1\. Access Actimize.
2\. Go to Research \> Transaction Investigation Module.
3\. Type the account number.

4\. Click Search.
Step 3
1\. Locate the alerted transactions.
2\. Select the WI ID.
Step 4
Did the Customer initiate the transactions?
1\. Ask the Customer to confirm the wire details (amount and recipient).
◦ Cancel the request if the Customer needs to change the wire amount or
Yes recipient (follow Customer Cancellation Requests, if appropriate). They must
submit a new request with the new details.
2\. Go to the next step to close the alert as Closed Non\-Fraud.
1\. Handle the account as Account Taken Over (ATO).
No
2\. Go to the next step to close the alert as Closed Fraud.
Step 5
1\. Click Next Steps and select the applicable closure action. Refer to the Alert Closure
Matrix.
2\. Select the applicable Reason. Refer to the Alert Closure Matrix.
3\. Add Notes (include any Lexis Nexis report ID).
4\. Click OK.
5\. Click the Navigate Back To arrow.
Step 6
1\. Go to Fraud Account Take Over (ATO) \- Amex Checking Fraud to resolve or rule out any
ATO concerns.
2\. Create an nGage case to capture any confirmed fraud activity, if applicable.
Step 7
1\. Repeat steps for all Transactions At Risk items until all are closed.
◦ Retail Monetary Activity ACH Same Day alerts: Work all same day ACH items
before working party level alerts that are non\-same day ACH.
2\. Go to the Retail Party Activity or Deposit Account Activity screen.
3\. Click Next Steps and select the appropriate action. Refer to the Alert Closure Matrix.
◦ If at least one Transaction At Risk item is closed fraud, close the Retail Party
Activity alert as Fraud.
4\. Select the applicable Reason. Refer to the Alert Closure Matrix.
5\. Add Notes (include any Lexis Nexis report ID).
6\. Click OK.
7\. Add notes in MBP BOUI indicating the outcome of your review and any actions taken.
8\. Click the Navigate Back To arrow.
", "

Modify closed alerts
Note: A second alert cannot be opened on a transaction that was previously alerted.
Step 1
1\. Access Actimize
2\. Go to Research, Transaction Investigation Module.
3\. Enter the account number.
4\. Click Search.
Step 2
1\. Locate the transactions previously alerted.
2\. Select the WI ID.
3\. Click the footsteps icon next to the Next steps drop\-down menu.
Note: The Next steps drop\-down menu is greyed out because the alert is already closed.
Step 3
1\. Select the Reset To: Ready from the Next Step drop\-down menu.
2\. Click OK.
Step 4
1\. Click on the Item ID.
2\. Click Next Steps from the drop\-down.
3\. Select In Process, if not already selected.
Step 5
Go to step 7 of Review Alerts section.
", "
Create new alerts
Note: A new alert should only be created for a transaction not previously alerted. Transactions
that did not generate an alert systematically in Actimize, will have already been approved.
Step 1
1\. Access Actimize
2\. Go to Research, Transaction Investigation Module.
3\. Enter the account number.
4\. Click Search.
Step 2

1\. Checkmark all the individual transactions that are confirmed fraud.
◦ Note: If an existing WI ID is present, an alert already exists and a new alert for that
transaction cannot be created.
2\. Click Create New Alert.
Step 3
1\. Click on the Item ID.
2\. Click Next Steps from the drop\-down.
3\. Select In Process, if not already selected.
Step 4
Was the new alert created for a check deposit item?
1\. Go to Next Steps \> Reject Manually in ImageCenter.
2\. Select the most relevant reason(s). Only use Other in scenarios where no other
reason is applicable.
Yes
3\. Add Note in Actimize for Reason(s) that indicate a detailed note is required.
◦ Note: Do not use pipe \|\| characters in Add Note.
4\. Click OK.
1\. Go to Next Steps \> Closed Fraud.
2\. Select the most relevant reason. See Alert Closure Matrix below.
No
3\. Add Notes, including any Lexis Nexis report ID.
4\. Click OK.
", "
Fraud Monitoring (M\-Sat)
Step 1
1\. Access Actimize.
2\. Go to Settings \> Platform List.
Step 2
1\. Select High Focus Customer.
2\. Click New Item.
Step 3
1\. Select Party Key and type 5201 followed by the Organization Customer ID from MBP
BOUI. For example, 5201\.7XXXXXXXXXX.
2\. Click Save.
Customers added to the High Focus Customer list will have Actimize alerts generated for all
ACH, wire, and check activity.

Step 4
1\. Access the account in MBP BOUI.
2\. Place the necessary informational restriction in MBP BOUI.
Fraud Monitoring \- use when account activity should be watched to track patterns of fraud for
investigation with a 30\-day expiration.
", "
Customer Cancellation Requests
Step 1
1\. Access Actimize.
2\. Go to Research \> Transaction Investigation Module.
3\. Type 5201\. followed by the Organization Customer ID from MBP BOUI in Party Key. For
example, 5201\.7XXXXXXXXXX.
Click Search.
Step 2
1\. Locate the transaction the Customer is requesting to cancel.
2\. Is there an alert captured for the transaction?
◦ An alert will be identified with a WI ID.
YesGo to the next step.
Advise the Customer that the transaction has already been processed and cannot be
No cancelled.
Process complete.
Step 3
Does the WI Step indicate Ready or In Process or Pending Review?
Advise the Customer that we will attempt to cancel the transaction but cannot guarantee.
Yes
Go to the next step.
Does the WI Step indicate Closed â€“ Non Fraud?
• Yes: Advise the Customer that the transaction has already been processed and cannot
No be cancelled.
• No: Advise the Customer that the transaction will be cancelled. Go to applicable
procedures to resolve any fraud concern.
Process complete.
Step 4
1\. Click the hyperlinked WI ID.
2\. Click Next Steps from the drop\-down.

3\. Select In Process, if not already selected.
4\. Assign to yourself for immediate review. Do not assign an item to yourself unless you are
available to work it immediately:
◦ Click the checkbox next to your alert.
◦ Click Assign (near top of Actimize window).
◦ Select Assign to me in dialog box.
◦ Select OK.
Step 5
1\. Access the Transactions At Risk section.
2\. Click the check box next to each Item ID. (If more than 3 must select Show all)
3\. Click Actions.
4\. Select Change Step and click Execute.
5\. Select In Process as Next Step.
6\. Click Ok.
Step 6
1\. Select Operational Error as Reason.
2\. Click OK.
3\. Click Navigate Back To arrow.
Step 7
1\. Repeat steps 5\-7 for all Transactions At Risk items until all are closed.
2\. On the Retail Party Activity or Deposit Account Activity screen, click Next Steps from
the drop\-down.
3\. Click Next Steps from the drop\-down and select Unknown as closure action.
4\. Select Operational Error as Reason.
5\. Click OK.
6\. Leave notes in MBP BOUI on the Customer/organization level, indicating the outcome of
your review and any actions taken.
7\. Click Navigate Back To arrow.
", "
Alert Closure Matrix
Closure
Actimize Closure action
Closure action Closure reason reason
queue definition
definition
Evidence
from fraud
review
Outcome of fraud
concludes no
review results in no
Retail Party fraud
Closed non\-fraud fraud concerns. No fraud
Activity concern, but
Result: Transaction
Customer
will be processed.
has not been
contacted to
confirm.

No Fraud \-
Customer has been
Activity
contacted and confirmed
confirmed by
no fraud concern.
Customer
Possible uses: duplicate
Operational transaction, tech error,
Error: Do not Customer request to
use cancel, account is
restricted or closed.
Other: Do not
Do not use
use
Evidence that a
Outcome of fraud review
true
results in definitive
Account Takeover Customerâ€™s
Closed fraud confirmed fraud.
Fraud account has been
Result: Transaction will
taken over by a
not be processed.
fraudster.
Evidence that a true
Business Email
Customer is a victim of
Compromise /
business email
Scam / Social
compromise, scam, or
Engineering
social engineering fraud.
Evidence that a true
Customer is intentionally
First\-Party
engaging in fraud activity
Fraud
for the benefit of
financial gain.
Evidence of kiting fraud
where a Customer may
take advantage of funds
Kiting Fraud
availability to make use
of non\-existent funds
expected to return later.
Evidence that an account
Synthetic was opened fraudulently
Identity / using false or a
Fictitious combination of true and
Identity false identity
information.
Outcome of fraud review Evidence that a
is inconclusive to true
Suspected confirm fraud, but fraud Account Takeover Customerâ€™s
Fraud concerns are still present. Fraud account has been
Result: Transaction will taken over by a
not be processed. fraudster.
Evidence that a true
Business Email
Customer is a victim of
Compromise /
business email
Scam / Social
compromise, scam, or
Engineering
social engineering fraud.

Evidence that a true
Customer is intentionally
First\-Party
engaging in fraud activity
Fraud
for the benefit of
financial gain.
Evidence of kiting fraud
where a Customer may
take advantage of funds
Kiting Fraud
availability to make use
of non\-existent funds
expected to return later.
Evidence that an account
Synthetic was opened fraudulently
Identity / using false or a
Fictitious combination of true and
Identity false identity
information.
Possible uses:
Outcome of fraud review
duplicate
results in no fraud
transaction, tech
concerns, but there are
error, Customer
other reasons to prevent
request to cancel,
transaction processing.
account is
For example, customer
Unknown Operational Error restricted or
requests to cancel, or
closed.
transaction restriction is
present on account.
The specific
Result: Transaction will
reason for using
not be processed.
this closure action
must be
thoroughly

