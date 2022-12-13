# IA - Version Change Log

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
