The test addin was created using "yo office" generated per https://learn.microsoft.com/en-us/office/dev/add-ins/quickstarts/outlook-quickstart-yo then modified for multiselection.

Classic Outlook on Windows
Open Classic Outlook
Create a folder in your inbox calld "testing folder"
copy one email into that folcer and past it 10 time, select all in the folder and copy and paste 20 times. There will now be 200 items in that folder.
Close Outlook Classic
start a command prompt
cd to folder of addin - TestSelectionAddin (c:\addintest\TestSelectionAddin on my machine)
run "npm start" from command line
When Classic Outlook luanches, click on the Show Taskpane button.
Repro time...
Be sure teh addin "Show Taskpan" button" is showing.
Select 100 items - it Can select 100
Click on the "Get information" link - it will count the items selected.
No error thrown.
Select 101 items and the addin is disabled.
run "mpm stop" to stop debugging
Close Classic Outlook

New Outlook Test on Windows:
Open New Outlook
Create a folder in your inbox calld "testing folder"
copy one email into that folcer and past it 10 time, select all in the folder and copy and paste 20 times. There will now be 200 items in that folder.
New Outlook Classic
start a command prompt
cd to folder of addin - TestSelectionAddin (c:\addintest\TestSelectionAddin on my machine)
run "npm start" from command line
When New Outlook luanches, display the Show Taskpane addin.
Repro time...
Be sure teh addin "Show Taskpan" button" is showing.
Select 100 items - it Can select 100
Click on the "Get information" link - it will count the items selected.
No error thrown.
Select 101 items and the addin is disabled.
run "mpm stop" to stop debugging
Close New Outlook

OWA test on Windows:
Have done the abobve tests prior, so the addin will show in OWA.
Repro time...
Be sure teh addin "Show Taskpan" button" is showing.
Select 100 items - it Can select 100
Click on the "Get information" link - it will count the items selected.
No error thrown.
Select 101 items and the addin is disabled.
 

