## SD Stores Returnables Releases

### 1.1.1

#### Enhancements

- When the Generate Penalty Charge Invoice process is run, additional information is now stamped in the invoice lines. Additional lines with Item No, Serial No, Original Order No. and Original Invoice No are added.

- Changes were made to the logic of the ‘Generate Penalty Charge Invoice’ function.

- Changes were made to the SD Packaging Control Ledger - actions were renamed on the ribbon and fields in the list were renamed.

- A new field 'Penalty Charge in Separate Invoice' was added to the Setup Card. If set to Yes, then the late penalty charge is not included in the Sales Return Order and the Sales Return Order will contain only a line with returnable packaging.

### 1.1.0

#### Enhancements

- Made changes to ensure that the charge Model Code is updated for Open Package Ledgers when changed on Item Setup.

- Added functionality to define and apply Damage and Non Return charges.

- Functionality was added to allow charges to be defined at custom period lengths and amounts.

### 1.0.0

#### Enhancements

- Functionality for Returnable Packaging Charge Models was created.

- Made a change that if a customer books a larger quantity than is returned then the system should clear the collection date, book returned date and the return order no from the pack ledger entry.

- For visual consistency the actions in the Actions tab were placed in the same groups as on the Home tab on the Returnable Packaging Setup Page.

- The About Page was reordered to the correct position in the product's object list.

- Visual changes were made to the Returnable Packaging Activity Group Page.

- Made a change that when posting the return order for the return packaging, the apply to document should be the original invoice.

- Changes were made to the reverse function when called from the packaging history.

- Made a change to clear the collection date from the return package ledger entries when the return order is deleted.

- Made a change to the functionality to allow instances where the site doesn't know the exact quantity of returnable items that will be there when they go to collect them. Now the system handles when more returnable packaging items are added manually to the sales return order and when less returnable packaging items are returned and updates the history accordingly.

- Separate lines are now created for each returnable package unit even when there are no  serial nos.

- Made a change to the Return Package Ledger Entries when processing returns and the Booked return date is not filled in to default the Booked return date to Collection Date = Workdate.

- A popup window was added to allow the user enter what date to calculate the penalty charges. Extra logic was also added to check and calculate for any lines with a Return Due Date < Booked Return Date.

- Made a change to allow users change the Return Package QC Code on the lines from a drop down list.

- Changed the logic of the reverse process for posted return packages to copy everything as per a copy doc function.

- The objects were renamed from a prefix of SD-RP to SD-RS.

- The objects version list was stamped to include the new name of the object.

- Created a Generate Interim Billing routine from the Return Package Ledger Entry. Allow users option to choose the calculation date and the posting date.

- Created a process for returnable packaging where the shipped quantity is more than one in one line.

- Posted credit memos for returnable packaging is now applied against the original invoice.

- In the Returnable Package Ledger Entries, allow users to choose the Return Package QC Code from a drop down list only and not allow users to type a new code.

- Allow recalculation of penalty charges even if the booked return date has been entered. Functionality was added to create a popup to allow the user to enter the date at which to calculate the penalties.

- A change was made to copy over the Ret.Packaging due date calculation to the Ret.Packaging Item Setup.

- The return package tracking level was removed from the Setup Card. Tracking is now defied on the item.

- Made a change to ensure that penalty charge is only calculated if the Booked Return Date is blank or the Booked Return Date is greater than today.

- Created functionality to return the packaging deposit.

- Added explanation on the line to explain the penalty charge amount added.

- Added the Penalty Charge Last Calc Date field to check when the Penalty Amount was last calculated.

- A change was made that when creating a Return Order, the Order Date is the Booked Return Date and the Posting Date is the Collection Date.

- Made a change to filter the Add Returnable Packaging Items action on the Returnable Packaging Item Setup Card.

- Reviewed and refactored code changes.

- Visual changes made to the Returnable Packaging Ledger page.

- Made visual changes to the Returnable Packaging Item Setup list page.

- Made visual changes to the Returnable Packaging Setup Card.

- Visual changes were made to the Role Centre to bring it in line with our other ISV products.

- Our standard About Page was created and surfaced on the SD Stores Manager Returnable Packaging Role Centre and Setup.

- Standard NAV OneNote, Notes and Links Actions were from the following pages: Ret. Packaging Setup, R.Package Item Setup, Ret. Package History, and Ret. Billed Entries.

- The objects were renamed to reflect the naming convention of our other ISV products.

- The Version List for the objects were stamped as per our ISV conventions.

- Reordered and renumbered objects.

- Code initially reviewed and versioned.

- Added a reverse process to allow processed ledger lines to be reversed out to the QC location.

- Created an event to ensure that the package ledger record is updated when the return order is deleted.

- Made changes to the Returnable Packaging Activity page which included adding KPIs to the page.

- Created a Factbox per item and per customer and added to the History pages.

- Created a Factbox per item and per customer and added to the Packaging Ledger.

- Created a new Statement of Charges Report that details the charges and what packaging is outstanding that makes up the charges.

- Created a Sales Order returnable packaging factbox.

- Made a change to allow for a penalty on late return by packaging type.

#### Bug Fixes

- A fix was made to remove package ledger entries when a standard corrective credit memo is created and posted. 

- An issue was fixed with the recalculation logic in the returnable packaging ledger.

- Fixed an issue where the return package ledger entry lines were not split into separate lines.

- A fix was made where corrective credit memos created for invoices with returnable packaging were not deleting the associated entries from the return package ledger entries.

- Fixed an issue where the return package ledger list the relation with the interim billing invoices.

- Fixed an issue where the return due dates on the return package ledger entries were different for the same shipment.

- Fixed an issue with the Penalty Amounts calculations.

- Fixed an issue where a sales order for two return package items with serial numbers was created and posted and, in the return package ledger, two entries with different return due dates were created for the same shipment.

- Issues were fixed with the Interim Billing where the data was not cleared if the credit memo was deleted.

- A fix was made to take standard corrective credit memos into account for return packaging. When a corrective credit memo is created for an invoice with returnable packaging, the ret.package ledger entries should be deleted when the credit memo is posted.

- An issue was fixed where, if the user continually selected the Process Packaging Returns Action in the Return Package Ledger, new Sales Return Orders were being continually created.

- The description for the penalty charge was updated and formatted correctly on the generated Sales Return Order.

- Fixed an issue where the hierarchy for pricing the returnable item in the return order was not correct,

- Fixed a typo in the Return Package Ledger.

- Fixed an issue where the booked return date in the Return Package Ledger was overwritten when using the Process Package Returns.

- Fixed an issue with calculating the penalty charges.

- Fixed an issue where the serial number was not assigned to the Sales Order Return Line.

