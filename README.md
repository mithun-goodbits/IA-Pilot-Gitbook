# IA - Version Change Log

#### Change log - Version 1.2.3

<details>

<summary>Distribution Information text for CPU value predicted files</summary>

01 August 2023

1. Predict certain spreadsheet's CPU value and if predicted, will show a text in the user dashboard for the user to check for distributions.

</details>

<details>

<summary>Handling known password-protected spreadsheets</summary>

01 August 2023

1. Added an input box for adding the password in the Hot queue and edit section
2. By using the added password IA will process the protected sheet.

</details>

<details>

<summary>Search panel improvements by edited fund tag</summary>

01 August 2023

1. Added a dropdown for Edited Fundtag search in the main search panel

</details>

<details>

<summary>Displaying Mime type in the user dashboard</summary>

01 August 2023

1. Every original attachment has the mime type displayed in the user dashboard.

</details>

<details>

<summary>Input field for adding spread value in the System wide universal settings section</summary>

01 August 2023

1. In the “System-wide universal settings” section added new a field where the spread value can be changed.
2. The error description for SE5021-23 will change according to the variable field.

</details>

<details>

<summary>Bulk uploading update feature</summary>

01 August 2023

1. Bulk uploading where updating a record if all the fields match then it can still accept the new records that had not been entered yet.

</details>

<details>

<summary>Change the color scheme of Review</summary>

01 August 2023

1. Changed SE5031 Color review from Red to another color scheme

</details>

<details>

<summary>Update the published product details on the Sender management page while doing manual upload</summary>

01 August 2023

1. Products from Manually uploaded files should show up in the sender management/product listing page after successful publishing

</details>

<details>

<summary>Bug Fixes</summary>

01 August 2023

1. Fixed SE5029 error code is not working properly issue

</details>

#### Change log - Version 1.2.2

<details>

<summary>Change logic of SE5021,SE5022 and SE5023</summary>

18 July 2023

1. Changed the Logic of SE5021, SE5022, and SE5023 errors.
2. When IA predicted 2 prices say VALUE A and VALUE B.\
   If |VALUE A-VALUE B| divided by MIN(VALUE A, VALUE B) \* 100 >= **Chosen spread value** then we are showing errors based on the Value A and Value B

</details>

<details>

<summary>Add an indication in the UI for the files that are ignored in processing</summary>

18 July 2023

1. Added text in the email summary section to indicate that the file is ignored while processing.

</details>

<details>

<summary>Start resolve button for Review status email attachments</summary>

18 July 2023

1. Added a new status called "Review" For Asset allocation emails.
2. Added Start resolving functionality for asset allocation emails.

</details>

<details>

<summary>Bug Fixes</summary>

18 July 2023

1. Fixed the Inactive products not able to be resolved by Resolve all option.
2. Included an extra space before appending the resolving text for SE5028 and W3006 errors.
3. Fixed the bug in the force publish section(getting future date error while doing force publish).

</details>

####

#### Change log - Version 1.2.1

<details>

<summary>Add a button to download Standard IMD unit price sheet format</summary>

12 July 2023

1. Added a button to download the Standard IMD unit price sheet format with auto-populated data

</details>

<details>

<summary>Implemented Force Publish feature </summary>

12 July 2023

1. Force Publish feature implemented for IA generated error (SE5028) to handle resolve feature

</details>

<details>

<summary>Add the additional fields in the bulk upload template in product add section</summary>

12 July 2023

1. Added the following additional fields in the bulk upload template
   * Self-publisher select field
   * Private select option

</details>

<details>

<summary>Bug Fixes</summary>

12 July 2023

1. Fixed the Emails that are being predicted with reverse dates issue.
2. Fixed A particular fund-size email had 3 attachments, yet the IA only processed one issue.

</details>

<details>

<summary>Integration of Asset allocation files processing</summary>

12 July 2023

1. Integrated Asset allocation file Processing

</details>

#### Change log - Version 1.2.0

<details>

<summary>Update the list of ignoring tabs</summary>

05 July 2023

1. Ignored tabs in the sheet which is having the following names&#x20;
   * Paste Here
   * DATA
   * NAV Spread

</details>

<details>

<summary>Bug Fixes</summary>

05 July 2023

1. Internal Server issue while doing the resolution of W3006 error

</details>

<details>

<summary>HP Status for the Fund size files</summary>

05 July 2023

1. Added the functionality of HP status for the Fund size files.

</details>

<details>

<summary>Logic can be updated when handling invalid date fields(422 Errors)</summary>

05 July 2023

1. If a file contains entries without dates that coincide with entries with (CUM) and (EX) highlighted in the date will create a separate file with an Invalid date error.

</details>

<details>

<summary>Future date Logic change based on past and future date in file</summary>

05 July 2023

1. If we have a future date in a file we will split the files according to past and future dates. So that we will generate 2 files
   * one is for past(including today) and this will publish to the blockchain
   * other is for future dates, it will show a future date error

</details>

<details>

<summary>Functionality of when we encounter W3006 future date errors</summary>

05 July 2023

1. Created a separate email entry while resolving W3006 errors.

</details>

#### Change log - Version 1.1.9

<details>

<summary>Fund size file Integration</summary>

26 June 2023

1. Added a new model for Fund size integration.
2. Completed the fund size file processing

</details>

<details>

<summary>Celery task to Lambda Function Migration</summary>

20 June 2023

1. Updated the existing Celery tasks to the Lambda functions.

</details>

<details>

<summary>Integration of New Prediction Models </summary>

20 June 2023

1. Added an improved Unit price model.
2. Added a new Fund tag prediction model based on the file's data.

</details>

#### Change log - Version 1.1.8

<details>

<summary>Changed the text Fund Tag text from "Detailed Asset Allocation" to "APRA 533 Asset Allocation".</summary>

23 May 2023

1. Changed the naming of the "Detailed Asset Allocation" to "APRA 533 Asset Allocation" for the new fund tag model in the pilot when predicting the APRA AA.

</details>

<details>

<summary>Included all IA SE errors in the main search panel, such as the categorized ones (eg SE5001 for HOTQUEUE, SE5004 for EWOA etc)</summary>

23 May 2023

1. Previously, in the Iress user dashboard search panel, we are not displaying categorized errors. So Included all the IA SE errors in the main search panel.

</details>

<details>

<summary>Bug Fixes</summary>

23 May 2023

1. Fixed the Delete functionality which was not working properly.

</details>

#### Change log - Version 1.1.7

<details>

<summary>For sender management - add another column to identify the data type for each type of file</summary>

17 May 2023

1. For sender management added another column called Data Type and auto populated for the existing ones

</details>

<details>

<summary>Bug Fixes</summary>

17 May 2023

1. When enabling Start Working and then disabling start working, the workflow status changed to ERROR rather than reverting back to QUARANTINE.

</details>

#### Change log - Version 1.1.6

<details>

<summary>Changes in UI for Quarantine Emails</summary>

15 May 2023

1. Move the Quarantine option on the ribbon to under the Others section
2. Include a start resolving button to Quarantine (can keep the existing delete button)

</details>

#### Change log - Version 1.1.5

<details>

<summary>Add a start working button to SE5012 "Inactive Product"</summary>

08 April 2023

1. Added start resolving button for Inactive products

</details>

<details>

<summary>Bug Fixes</summary>

08 April 2023

1. Time zone changes affecting the email analysis - "no action" required email count to be updated.
2. SE5014 "Not a Product" errors are missing the sheet name to identify which tab in the spreadsheet the error came from.

</details>

#### Change log - Version 1.1.4

<details>

<summary>External link to emails</summary>

17 April 2023

1. Added a textbox in the Individual user settings page
2. Added the redirection towards the delegated Gmail inbox when the open link is clicked on the email detail section

</details>

<details>

<summary>Corrupted File Processing</summary>

17 April 2023

1. Fixed the Corrupted file issue.

</details>

#### Change log - Version 1.1.3

<details>

<summary>Cumulative Graph Changes</summary>

04 April 2023

1. Updated the cumulative graph to display and provide statistics on “ no action required” emails satisfying the below conditions.
   * Only published status workflows in the email.
   * Only HP status workflows in the email
   * Combination of either published and HP statuses only in the email.

</details>

<details>

<summary>Starred options box be bought to the closest foreground</summary>

04 April 2023

1. Stared options box moved to the closest foreground so the entire box can be seen so that you do not need to scroll to see the cancel, remove star, update options

</details>

<details>

<summary>Warning text changes for email analysis</summary>

04 April 2023

1. Changed the warning text to "IA was not introduced yet. Data Unavailable"  If the date selected is before 05 Dec 2021 (When IA first became live in production). Same should apply to the weekly and monthly selection.
2. Changed the Warning text to "Cumulative stats not available during this timeframe" if the selected date range is before 03 Feb 2023.
3. On dealing with the overlapping dates where calculation uses partial data IA will show the warning message as "Data might be inaccurate".

</details>

#### Change log - Version 1.1.2

<details>

<summary>Increase the size of the email label name up to 225</summary>

24 February 2023

1. Increased the Label name text field size up to 225 characters

</details>

<details>

<summary>Changes in Product edit Popup</summary>

24 February 2023

1\. Static data is added to a separate tab in the Add and edit product section



</details>

<details>

<summary> IA- Admin Dashboard- Code optimization to reduce loading time</summary>

24 February 2023

1.Convert from ORM queries to direct DB queries



</details>

<details>

<summary>Show all error codes/warnings search options on the Main Search panel</summary>

24 February 2023

1. Added new error codes in the Main search panel for 422,500,502,504 errors

</details>

<details>

<summary>Auto tagging yourself on the manual upload option / fixing W3006 </summary>

24 February 2023

1. Added Auto-tagging functionality while doing the manual upload and resolving the W3006 errors.

</details>

<details>

<summary>Feature to turn on/off auto-tagging</summary>

24 February 2023

1\. Added an auto-tagging on/off feature on the settings page



</details>

<details>

<summary>Settings Page Modification</summary>

24 February 2023

1. Changed IA Settings Page to Restrict universal settings only to super admin

</details>

<details>

<summary>Label Creation</summary>

24 February 2023

1. Added the functionality for the user should be able to create the labels against each email in the user dashboard.

</details>

<details>

<summary>Product Lookup redesign </summary>

24 February 2023

1. Added a separate tab on the product lookup and Add/Edit product page to display the static data coming from the blockchain.

</details>

<details>

<summary>Merge the Cumulative email analysis and Email analysis on one page</summary>

24 February 2023

1. Merged the Cumulative email analysis and email analysis pages as one page and kept the name of the page as Email analysis.
2. Added “N/A” value for the items in the email analysis section while the stats selected a date range before 02 Feb 2023.

</details>

<details>

<summary>Bug Fixes</summary>

23 February 2023

1. Email doesn't show the chevron icon to show all the attachments to the mail

</details>



#### Change log - Version 1.1.1

<details>

<summary>Product Lookup redesign</summary>

09 February 2023

1. Added table view in the graph section.
2. Added more product-related details.

</details>

<details>

<summary>Changes in Product Add and edit Popup</summary>

09 February 2023

1. Added more product-related fields in the Product add and edit popup sections.

</details>

<details>

<summary>Product management - self-publisher, private product</summary>

09 February 2023

1. Added Self-publisher and private checkboxes in the Product add popup.

</details>

<details>

<summary>Show Repair queue error messages in the email summary section</summary>

09 February 2023

1. If there are warnings and repair errors for an email, should display the repair queue error messages in the email summary section.

</details>

<details>

<summary>Change in tag notification text</summary>

09 February 2023

1. Changed the sentence to \[Tagger] tagged you, \[+ other Tagged Users] in the mail. Reason being \[Reason]

</details>

#### Change log - Version 1.1.0

<details>

<summary>Performance Improvements</summary>

01 February 2023

1. User Dashboard optimization completed
2. Added new check in refresh logic on the user dashboard section
3. Optimized the workflow analysis section.

</details>

<details>

<summary>Bug fixes</summary>

01 February 2023

1. Instead of showing EWOA status, the emails that come under hot queue mail should show up in the Hot queue status.

</details>

#### Change log - Version 1.0.9

<details>

<summary>Settings Page Improvements</summary>

19 January 2023

1. Added the following headings System wide universal setting, Individual User Settings in the Settings page.

</details>

<details>

<summary>Reports Page Improvements</summary>

19 January 2023

1. Added No action required and no of email count while hovering over the data visualization bar.

</details>

<details>

<summary>Performance improvements</summary>

19 January 2023

1. Optimized the APIs in the trend analysis section to improve the performance of the application.

</details>

#### Change log - Version 1.0.8

<details>

<summary>User dashboard- added a refresh button to fetch new emails</summary>

11 January 2023

1. Added the functionality of enabling a refresh button only when there are new emails

</details>

<details>

<summary>Limits updation from the Settings page</summary>

11 January 2023

1. Price limits for nav\_a, entry\_a, and exit\_a are added to the settings page.
2.  Price limits can be updated universally, and not for individual senders from Settings Page.



</details>

<details>

<summary>Web application optimization tasks</summary>

11 January 2023

1. Reduced the user dashboard loading time
2. Changed the direct DB queries for the metrics portion in the admin dashboard.

</details>

<details>

<summary>URLs in the Hot queue notes and instructions section.</summary>

11 January 2023

1. Added the ability to copy the notes and instructions in the hot queue popup in the user dashboard.
2. Added the ability to view the URLs if any in notes and instructions.

</details>

<details>

<summary>Added time intervals</summary>

11 January 2023

1. Added time intervals in the x-axis point for all the graphs having time
2. Changed the x-axis in the form 12 am - 1 am instead of just 1 am

</details>

<details>

<summary>Bug fixes</summary>

11 January 2023

1. In the User dashboard, the Tagged user list is not showing correctly

</details>

#### Change log - Version 1.0.7

<details>

<summary>Error Text Updation</summary>

13 December 2022

1. Updated the error code text  SE5024, SE5025, and SE5026 to "For the product (Fund name), Predicted \_\_\_\_ is greater than XXXX"

</details>

<details>

<summary>Notification Improvements</summary>

13 December 2022

1. Removed the cross button for deleting the notifications.

</details>

<details>

<summary>Settings Page Modification</summary>

13 December 2022

1. Updated the tagged user dropdown list to be individual
2. Added infinite scroll to user dropdown
3. Updated the Preference to only show the selected users in the drop-down list\


</details>

<details>

<summary>Displaying the Processed Sheet Name</summary>

13 December 2022

1. Displayed the Spreadsheet's processed Tab(sheet) name for each processed file- on the details pane.

</details>

<details>

<summary>Overview>Metrics- The number against Repair queue changes to 0</summary>

13 December 2022

1. The number against the Repair queue is now fixed even if the status is changed to resolved.

</details>

#### Change log - Version 1.0.6

<details>

<summary>Naming Convention for Bulk Downloaded Files (product details)</summary>

09 December 2022

1. When the search field is blank, then the download option downloads all products to a file called IA PMDB Products All \_downloaded date-24hrtime.csv
2. Otherwise, it downloads the products that match the search to a file called IA PMDB Products Search by xxxxxx\_downloaded date-24time.csv

</details>

<details>

<summary>Manual Upload Improvements</summary>

09 December 2022

1. Added the ability to view the list of selected files, and add/remove files from the list

</details>

<details>

<summary>Info against settings items</summary>

09 December 2022

1. Settings page- added an information button against all items in the settings page, and display information regarding that setting when clicked.

</details>

<details>

<summary>Tagged user list selection</summary>

09 December 2022

1. Settings page- Added the ability for the user to set a list of users, who should be showing up on their starred emails filter

</details>

<details>

<summary>Watch Expiry Alert</summary>

09 December 2022

1. Created an alert for when the watch expiry is in less than 6 days

</details>

<details>

<summary>Additional Identifier in the product detail section</summary>

09 December 2022

1. Added the ability for users to add additional identifiers (in addition to the primary identifier) in the product details section.

</details>

<details>

<summary>Mail detail section improvements</summary>

09 December 2022

1. The subject in the mail detail section is trimmed. This section should be dynamic when the user does resize the mail detail section.

</details>

<details>

<summary>Sender management pagination modification</summary>

09 December 2022

1. Sender management- Reduce the number of items per page from 100 to 25, to make the loading faster.

</details>

<details>

<summary>Change text for SE5024,SE5025,SE5026 Error codes</summary>

09 December 2022

1. Changed the error code text for SE5024, SE5025, and SE5026 error codes according to the value set from the Django admin section.

</details>

<details>

<summary>Bug Fixes</summary>

09 December 2022

1. Fixed the Emails received in the fund data mailbox that is sometimes not fetched by IA issue.
2. Incorrect HP error assignment on new products. (Different unique id, but same product name/sender product name )
3. IA is not fetching emails released from quarantine.
4. Click on a notification item with multiple files/errors. Upon resolving one, it goes back to the home page
5. The notification number is incorrect - When the user resolves one tagged email then the count of the notification section is reduced. Even though the mail gets resolved the count should not be reduced unless the user untagged that email from the user.
6. Fixed the EWKA error occurring for the Hot queued mail issue.



</details>

#### Change log - Version 1.0.5

<details>

<summary><strong>Search filter Modifications</strong></summary>

November 17, 2022

1. The user is now able to search the All with “Read”, and “Unread” combinations.
2. Added Read and Unread filter functionality with whole data.
3. The All checkbox will get dissected automatically when the user selects some specific date fields.

</details>

<details>

<summary><strong>Unwanted space removal</strong></summary>

November 17, 2022

1. Removed unwanted white space in product names published by Blockchain

</details>

<details>

<summary>Cumulative email analysis</summary>

November 17, 2022

1. Added cumulative email analysis section in the admin dashboard(Reports section).
2. The repair queue count in the cumulative email section will not change if an already existing error email item is resolved.

</details>

#### Change log - Version 1.0.4

<details>

<summary><strong>Search Filter Redesign</strong></summary>

November 14, 2022

1. Removed the locked dates for Read and Unread checkboxes.

</details>

<details>

<summary><strong>Blockchain Warnings</strong></summary>

November 14, 2022

1. Changed the W6003 warning from “Set to Repair Queue” to “Set to Republish”.

</details>

<details>

<summary>Notification Improvements</summary>

November 14, 2022

1. Added a refresh button in the notification section.
2. Added the refresh functionality while clicking on the notification bell icon.

</details>

<details>

<summary>Bug Fixes</summary>

November 14, 2022

1. Fixed the bug in the hot queue section. The bug was when clicking on either Notes or Instructions it results in a blank page.

</details>

#### Change log - Version 1.0.3

<details>

<summary>UI Updates- User dashboard</summary>

October 31, 2022

1. Included the logged-in user name next to the bell icon.
2. Added EWOA, Quarantine, and IA Processing statuses in the total breakdown section.
3. Updated the time with a leading zero for hours under 10
4. For unselected emails added a hint of a border
5. Changed the Selected emails are white, and items not selected are shaded.
6. Fixed at a certain number of characters of email address information.
7. Changed the sliders to adjust their respective window without adjusting the other window
8. Improved the design while resizing the User and Sender reports section.
9. White space after the subject line is removed.
10. The inconsistent height of the emails was removed.

</details>

<details>

<summary>UI Updates - Reports</summary>

October 31, 2022

1. File Analysis changed to Workflow Status Analysis. On Hovering over the title, the following text “Analysis of Workflow statuses predicted with a unit price fundtag” is added.
2. Product Analysis changed to Unit Price Records Analysis. On Hovering over the title, the following text “Number of individual records of products with unit price information and dates” is added.
3. On Hovering over the Files title, the following text “Processed files by IA predicted by IA with unit price fundtag” is added.
4. On Hovering over Workflow Status Analysis Emails, the following text “Total number of emails that have an IA unit price fundtag prediction” is added.
5. On Hovering over Files Emails, the following text “Total number of emails that have an IA unit price tag prediction but excluding emails that do not have any processed files such as Quarantine and EWOA” is added
6. On Hover over Files total, the following text “ Total is the number of files processed by IA. Total does not usually include Quarantine and EWOA as there are usually no files processed by IA for those" is added.

</details>

<details>

<summary>Sorting Improvements</summary>

October 31, 2022

1. Added sorting option for search results

</details>

<details>

<summary>Hot Queue- Notes and Instructions. </summary>

October 31, 2022

1. Added Notes and Instructions tabs
2. Updated the Character length of Notes and Instructions to 2000 Characters.
3. Added a pop-up while the user clicks on the hot queue status
4. Added the functionality to display remaining characters to reach the 2000 characters limit in HotQueue notes and instructions

</details>

<details>

<summary>Notification Improvements</summary>

October 31, 2022

1. In the notifications section, included the information about the user that Tagged the mail. eg: “Xxxxx Tagged you in the mail".

</details>

<details>

<summary>Search filter redesign</summary>

October 31, 2022

1. Changed the Tagged User Quick Search. While searching, it will show all the tagged items of the user/users selected without affecting the main search panel.
2. If users are already selected in Tagged User Quick Search and want to do a search in the main panel page, Then click on search in the main search panel, it will clear any users already in the Tagged User Quick Search before performing the search.
3. If the "all" checkbox is selected, then the date fields will get grayed, and added a text by saying "Unselect All to change date".

</details>

#### Change log - Version 1.0.2

<details>

<summary><strong>Feature 1: Notifications</strong></summary>

October 20,2022

1.Added Notification for the tagee when tagging email, include bell icon with number of starred/tagged emails for particular user

</details>

<details>

<summary><strong>Feature 2: Displaying the warnings</strong></summary>

October 20,2022

1**.**Displayed block chain warnings on successfully published emails/files.



</details>

<details>

<summary><strong>Feature 3: XLSM file processing</strong></summary>

October 20.2022

1.Added Support for XLSM file type (Excel Macro) processing in IA.





</details>

<details>

<summary><strong>Feature 4: Hot queue rules and notes</strong></summary>

October 20,2022

1.Hot queue- Added the ability for the user to add notes against each rule they create - notes are not mandatory.

2.Added the ability for users to view hot-queue rules and notes from the user dashboard, hot-queue tab







</details>

<details>

<summary><strong>Feature 5: Search filter redesign</strong></summary>

October 20,2022

1.Search filter redesign- Updated the Move read/unread filters inside the search pane.





</details>

<details>

<summary>Feature 6: Bulk product upload</summary>

October 20,2022

1.IA PMDB - Added the ability to bulk create products via CSV/xlsx file upload in prescribed format.



</details>

<details>

<summary><strong>Feature 7: Product download</strong></summary>

October 20,2022

1.Added the ability to download product information.



</details>

<details>

<summary><strong>Feature 8: Sorting</strong></summary>

October 20 ,2022

1.Added the ability for the user to sort the hot queue page - based on all columns displayed, in ascending and descending order.

2.Sender management- Added the ability to sort the list of senders based on all columns in ascending or descending order.



</details>

<details>

<summary>Feature 9: Products listing inside the sender profile</summary>

October 20,2022

1.Sender Management - listed the products which are successfully published by each sender inside the profile of the sender.



</details>

<details>

<summary><strong>Feature 10: Settings Page</strong></summary>

October  20 ,2022

1.Created a new Settings page



</details>

<details>

<summary>Feature 11: Manual Upload</summary>

October 20 ,2022

1.Added the ability to Manual upload more than 1 file at a time



</details>

<details>

<summary><strong>Feature 12: UI updates</strong></summary>

October  20 ,2022

1.Updated the UI of Product management page

2.Updated the UI of User management page

3.Updated the UI of Overview/Client reports

4.Updated the UI of Overview/User reports

5**.**Updated the UI of Overview/reports





</details>

<details>

<summary>Bug Fixes</summary>

October 20,2022

1.Removed the Image file from the Hot queue items in the dashboard

</details>



#### Change log - Version 1.0.1

<details>

<summary> Feature 1: Management </summary>

04 August 2022

1. Added a new Management button in the sidebar.
2. Changed the UI of the User management, Sender management, and Product management sections.



</details>

<details>

<summary>Feature 2: IA versioning and change-log</summary>

04 August 2022

1. Added the version in the pop-up on the left bottom logout section.
2. Added change log button on the logout section pop-up.

</details>

<details>

<summary>Feature 3: Product Lookup</summary>

1. Added Product lookup in the user dashboard sidebar.&#x20;

</details>

<details>

<summary>Bug Fixes</summary>

1. Fixed the Mails without attachments are not being considered in the hot queue item.

</details>

**Change log - 17 August 2022**

<details>

<summary><strong>Feature 1: Manual File Upload</strong></summary>

1. Added the ability for the user to upload csv / excel files via IA dashboard for processing.

</details>

<details>

<summary><strong>Feature 2: Turn IA On/Off (For updates etc)</strong></summary>

1. Added the functionality for the user should be able to turn IA on or off from the supervisor dashboard.
2. The user should be able to manually specify the time period from which the mails should be fetched.

</details>

<details>

<summary><strong>Feature 3: Admin and User Dashboard Improvements</strong></summary>

1. Update UI to resemble DDO- Implementation of sidebar and layout change on admin and user dashboards.
2. Changed the position of User Management, Sender Management, and Product Management on the sidebar**.**

</details>

<details>

<summary><strong>Feature 4: Hot Queue -  UI Improvements</strong></summary>

1. Changed activate/deactivate button to the green slide bar.

</details>

<details>

<summary><strong>Feature 5: Zip File Handling</strong></summary>

1. No passwords are required Zip files processing has been done.
2. Description has now changed for Zip files that have not been processed as an “Unhandled zip file”.

</details>

**Change log - 19 August 2022**

<details>

<summary><strong>Feature 1: UI Improvements</strong></summary>

1. User dashboard resizing the screens has been done.
2. Added the Error description in the error analysis section while hovering over a particular error code item.

</details>

**Change log - 22 August 2022**

<details>

<summary><strong>Bug Fixes</strong></summary>

Fixed the something went wrong error message issue.

</details>

####
