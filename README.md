# windows-to-ios-vcard
If you're interested in getting your Microsoft Outlook contacts to Apple iCloud contacts, you'll have to go through a little more work to get it done. Fortunately, the heavy lifting has been done for you!

First, export your Outlook contacts to CSV:

1. https://outlook.live.com/people/
2. Click on the "Manage" dropdown in the middle of the secondary top bar
3. Click on "Export Contacts"
4. Hit the "Export" button on the modal that pops up.
5. Save your csv file.

Next, download my helper spreadsheet: https://github.com/jeffrpowell/windows-to-ios-vcard/blob/master/contacts.xlsx

Then, use my contacts.xlsx file to help generate your iCloud compatible contacts:

1. Open up both your csv file and my contacts.xlsx spreadsheet 
2. Make sure the column headers in contacts.xlsx match the columns that Outlook supplied in your csv. If they aren't, you'll need to update my spreadsheet to match.
3. Paste the contents of your csv starting at A2 on the first worksheet tab. 
4. Flip over to the second worksheet tab
5. Copy the algorithms from row 2 down until all rows from the first worksheet are accounted for
6. Select all cells in the P column and copy them
7. Open up a blank file and paste the contents
8. Ctrl+h (find+replace)
   * "BEGIN -> BEGIN
   * END" -> END
9. Save the file as a .vcf file

You now have a valid contacts file that can be imported into iCloud!

1. https://www.icloud.com/#contacts
2. Click the settings gear in the bottom-left
3. "Import vCard..."
4. Find and select your .vcf file 
