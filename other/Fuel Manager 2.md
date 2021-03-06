Fuel Manager 2

Documentation

TransFlo Instruments Limited

Unit 6, Rose Lane Industrial Estate,
Lenham Heath, Maidstone, Kent,
UK. ME17 2JN.

Tel: +44 (0) 844 257 8181
Fax: +44 (0) 1622 859855

Introduction

The TransFlo FuelManager software package has been designed to provide the most efficient means of managing fuel stocks and vehicle fuel usage. It is designed to control and supervise single or multiple refuelling sites using the on site power of the range of TransFlo fuel dispensing systems.

This Manual is accessed via the FuelManager Application Interface and will run within you browser or alternatively is available as a PDF file that can be read from your Mobile Device/Tablet.

Main Control Panel

The Main Control Panel is shown below and is the main user-facing interface for the FuelManager application.

Main Control Panel

The Main Control Panel provides an easy means of navigating around the various facilities of FuelManager.  The command buttons are clearly labelled with their function. The command buttons are made available to suit the system configuration, for example the Data Transfer button is not enabled on a workstation not using the communication facilities. 


Vehicles/Plant 
Access to vehicle registration form and detailed vehicle records.

Drivers
Access to driver registration form and detailed driver records. Driver records can be password protected to conform with data protection legislation.

Product Storage Tanks
Storage tank details, stocks, dips, deliveries, etc.

Dispensing Pumps
Site pump details, throughput, totaliser readings, etc.

Fuel Order Entry
Entry of bulk fuel orders, editing of existing orders.

View Refuelling Transactions
Quick view of refuelling transactions.

Import Fuel Card Transactions
Entry of transactions purchased via fuel card.

Products
Fuel product names and codes.

Site Locations
Details of remote sites associated with your system.

Manual Transaction
Enter fuel purchased outside your system.

Data Transfer
Access to data communications facilities.

Reports
FuelManagers reporting facility.

Charts
Graphical representation of certain FuelManager data

Change Password
Change user password.

€ (Euro)
Conversion rate to be used by FuelManager.
Exit
Close FuelManager.

The date/time shown is taken from the operating system and is continually updated.

The functions are described below but all are not available to all users, also some are not available if unrelated to the current screen.

A standard menu may also show for some screens if relevant.

Save
Saves the current state of your database.

Print
Prints the active screen or report.

Sort Asc
Sorts data on the active screen in ascending order based on the marked field.

Sort Desc
Sorts data on the active screen in descending order based on the marked field.

Filter by Selection
Filters data on the active screen based on the marked field.

Apply Filter
Applies the last set of filter criteria to the active screen.

Remove Filter/Sort
Removes all filter and sort criteria.

Export to Excel
Enables the data source for the active screen to be exported to MS Excel.

Tools
Provides access to various database facilities, particularly the ability to export data to other MS Office family members, compact and repair the database and set up security accounts and permissions.

Set Links
The means by which FuelManager data is linked to all workstations.  This function is not normally required after initial commissioning and must be used with great care.

Refresh Links
A means of reconnecting any broken database links.

Exit System
Close FuelManager.

Vehicles and Plant
Note: The Vehicle Record screen is described in full in the next chapter (6).

Registering a vehicle or plant item.

Only enabled if Direct Polling is active.

The Vehicle Registration screen provides a quick and easy means of registering all your vehicles and plant items.  The information required about a new vehicle is kept to a bear minimum allowing changes to your fleet to be made quickly and simply.
To register a vehicle or plant item click on the Add Vehicle  button and complete the fields following the guidelines below:

Registration No.
This is a required field, maximum length 12 alphanumeric characters. Duplicates not accepted.

Identifier No.	Number shown on access device (RFID Tag etc.) Only required by remote system therefore any vehicles not directly using remote system can be left as the default of ‘0’. Duplicates not accepted except for ‘0’.

Fleet No.	Not required, for information and certain reporting functions only. Maximum length 12 alphanumeric characters. Duplicates not accepted.

Fuel Type	Required field, select from dropdown box.

Odo Type	Required field, select from dropdown box. If plant  selected odometer input will not be requested at time of refuelling.

Start Odo	Not required, most remote systems assume odometer entered at first refuelling is the Start Reading. However entering it may enable a more accurate start to your data collection.

Active	All newly registered vehicles are assumed to be active and therefore able to use the remote system to refuel.

Once you are satisfied with the information entered either tab to a new record or click the Add Vehicle button again, the new record is automatically saved.  
Remember that except for direct polling systems the new vehicle file must be uploaded to the remote site to enable refuelling.
The easiest way to select a particular record is to double click in the Registration No. field.

NOTE: FuelManager recognises certain reserved words entered as the first characters
in the Registration field as a prompt to distinguish special types of refuelling activity. Do not use
these words unless your system requires it, the TransFlo commissioning engineer will give advice.
The reserved words are: BOWSER, WORKSHOP, FUEL, SALES, MASTER. Their use is described later 
in this manual under the heading ‘Specialised Refuelling Activity’.

Blacklisting a registered vehicle

It may be necessary to blacklist a vehicle should its Identifier be lost and many other reasons. Once blacklisted and the updated vehicle file has been sent to the remote site that vehicle will be denied fuel at the pump.

The Active button indicates whether a vehicle is blacklisted. If YES it is active and can refuel. To change it’s state to NO select the relevant record and click on the Active  button.

Deleting a registered vehicle.

	Ensure that the relevant vehicle record is selected.
	Ensure the correct vehicle registration shows on the Delete button.
	Set the vehicle record as non-active. (NO shows on the Active  button).
	Click the Delete button.
You will be asked to confirm your action, once confirmed the vehicle record is immediately deleted from the database. However all refuelling transactions for that vehicle remain intact and can be reported on.

For direct polling systems the change is immediately effective however the deleted vehicle will still be able to refuel at remote sites until the new vehicle file is uploaded.

Change vehicle identifier number.

Should a vehicle identifier be lost, stolen or in any way made unusable it will be necessary to replace it and also ensure that an unauthorized person cannot use it.
This is easily achieved by issuing a new identifier and changing the related identifier in FuelManager.

You should ensure that there are no live transactions relating to the old identifier at any of your sites by initiating a communications Receive session. Any live transactions for the old identifier brought in after a change of Identifier number will not be posted but dealt with as Rejected Transactions.

	Select the vehicle record with the identifier to change.
	Click the Change Identifier button.
	You will be asked to confirm your action.
	Enter the new Identifier number, remembering that FuelManager will not accept duplicate numbers.

For direct polling systems the change is immediately effective, the new vehicle file must be uploaded to the remote sites.



Change Odometer.

	Allows easy changing of the Latest odometer reading of a vehicle.

	Select the relevant vehicle.
	Click the Change Odometer button.
	You will be asked to confirm your action.
	Enter the new odometer figure. (Affects Latest odometer field only).

NOTE: A start reading for a new odometer can be entered in the Start Odo field, this will set the Latest odometer field to the same value.  The Distance Life figure is not affected.

5.6 Last 7 days transactions.

A convenient means of quickly viewing all transactions for the selected vehicle that have occurred during the last 7 days.

Only transactions for the main vehicle fuel are shown, auxiliary products, e.g. Lube, are not displayed.

5.7 Messaging.

Sending a message to be displayed when a vehicle next refuels is available for systems where direct polling is employed only.

Click the Message button to enter a message for the selected vehicle.
Messages can be a maximum of 24 characters long.
Normally the message is removed once it has been displayed at the refuelling point, however by ticking the Repeat Message box it will continue to appear every time the vehicle refuels until the message is deleted at FuelManager.

Clicking the Active Message button will open a screen showing all messages currently in use. Messages can be deleted by marking them and clicking the Delete Records button.




5.8 Find vehicle.

The Find Vehicle feature provides a quick and easy means of locating a particular vehicle within a large vehicle database. It can be accessed from both the Vehicle Registration and Vehicle Record screens.


















Select vehicle here




The vehicle search is based on information available within the database relating to vehicle registration and/or fleet number.

To search for a vehicle enter as much detail as possible in the Registration / Fleet boxes.
Click Show Matching Vehicles.
Select your required vehicle by clicking on the left of the vehicle list. The selected vehicle is confirmed in the Selected Vehicle block.
Click Go To Selected Vehicle.
Vehicle search examples:

Entering ‘g’ (upper or lower case) in the Registration field and clicking Show Matching Vehicles will cause all vehicles beginning with ‘G’ to show on the list.
Entering ‘gb’ will restrict search to only vehicles with a registration beginning with ‘GB’ 
Entering ‘gb’ in the Registration field and ‘2’ in the Fleet field will restrict search to vehicles with a registration beginning ‘GB’ and a fleet number beginning with ‘2’.
Selecting Active or Non-Active rather than All will further restrict the search.

If both the Registration and Fleet fields are left blank the complete vehicle database is listed.

Clicking Go To Selected Vehicle will always close the Find Vehicle screen and return to the record selected on the screen that called it.

Clicking Exit will close this screen and return to the original record on the screen that called it.

5.9 Reports

Access to the Reports facility, which is described later in this manual.

6	Vehicle Record.

The Vehicle Record screen is accessed via the Vehicle Record button on the Vehicle Registration screen.

The Vehicle Record screen provides both a means of recording detailed information for each vehicle and showing the latest fuel and odometer statistics and cost data for each of the vehicle.

The fixed data for each vehicle is displayed across the top of the form. The status of the vehicle is shown bottom right as either Active: Yes or Active: No. You must return to the Vehicle Registration screen to change any of this data.



6.1 Vehicle statistics.

On the right of the screen is displayed a comprehensive list of vehicle statistics as held by FuelManager. This data is updated automatically by both automatic and manual refuelling transactions. 

6.2 Vehicle information.

The remaining fields on this screen are arranged into four sections and allow information to be entered providing a complete record for each of your vehicles. Although completing these fields is optional a number of them, if completed, can have an impact on either the refuelling operation of the vehicle or the reporting capability of FuelManager.

6.2.1 General information.

The general information relating to each vehicle is located in the block on the left of screen. 
The Cost Centre field can hold 12 alphanumeric characters and is used by the reporting facility to apportion fuel cost and usage to its cost centre.  A cost centre is typically a department, job or project with which the vehicles fuel costs are associated. There is no practical limit on the number of cost centres that can be used.
The action buttons to the right of the four date fields activate the FueManager calendar.

6.2.2 Ancillary fuel information.

Located in the block centre/top.
Odometer Limit is used by the remote island system to check the current odometer input at the time of refuelling. The odometer reading which is entered via the keypad on the remote system must be no less than the last reading and no more than the last reading + Odometer Limit. 
The Odometer Limit should therefore be set at the maximum distance a vehicle can travel on a full tank of fuel. 
If Odometer Limit is not entered the remote system uses a default of 9999.

Standard M.P.G. figure should reflect the expected average for the selected vehicle. A number of Reports use this figure to either highlight discrepancies or include/exclude vehicle records.

Tank Capacity limits the quantity of fuel that can be dispensed to the selected vehicle at each automatic refuelling as well as manual Transaction.
The default is 999.9 litres. The figure entered is in 1/10 litre, e.g. 1234 entered = 123.4 litres.

Auxiliary Tank Capacity and Fuel Name are required if the refuelling system at the remote site monitor fuel dispensed to secondary items, such as fridge units etc.

6.2.3 Allocating drivers to vehicles.

You can allocate two specific drivers to each vehicle. The drivers must be registered in the Driver section of FuelManager and must be Active.
This is generally used for information only.

Drivers are allocated by clicking on the action(search) buttons to the right of the driver fields. This opens the Find Driver screen from which you may make your selection by marking the required driver and then clicking the Go To selected Driver button.  Both the name and personnel number of the selected driver are displayed.

6.2.4 Unassigned fields.

The Vehicle Record screen shows four fields that are labelled Not Used. These can be altered as necessary to record any vehicle information of your choice. This may, for example, be tyre size, engine type etc.

To change the unassigned labels:

Double click anywhere within the field area associated with the label to be changed. 
Type the new label name in the Rename Field box and click OK.
These labels can be changed at any time and affect the record screen of all vehicles. When transactions are selected for report, by MS Excel for example, these fields are always referred to as Spare1, Spare2 etc. 

6.2.5 Memo

The Vehicle Record screen, as well as a number of other screens has a Memo facility attached to each record enabling notes relating to that record to be conveniently stored.



Drivers





					Only enabled if Direct Polling is active.

Note: The Driver Record screen is described in full in the next chapter (8).

7.1 Registering a driver.

The Driver Registration screen provides a quick and easy means of registering drivers.  The information required about a new driver is kept to a bear minimum allowing changes to your fleet to be made to be made quickly and simply.

To register a driver click on the Add Driver button.

Surname		This is a required field. Maximum 20 characters.

Personnel No.	This is a required field. Maximun 15 alphanumeric characters.

Identifier No.	Number shown on access device (RFID Tag etc.) Only required by remote system, therefore any drivers not directly using remote system can be left as the default of ‘0’. 
	Duplicates not accepted except for ‘0’.

Active	All newly registered drivers are assumed to be active and therefore able to use the remote system to refuel.

Once you are satisfied with the information entered either tab to a new record or click the Add Driver button again, the new record is automatically saved.  
Remember that except for direct polling systems the new driver file must be uploaded to the remote site to enable refuelling.

Blacklisting a driver.

The Active button indicates whether a driver is blacklisted,e.g. has permission the refuel. The button defaults to YES – active. To stop a driver from having access to the refuelling facility this must be set to NO. Change the state of the Active button by clicking on the button of the relevant driver.

7.3 Deleting a driver.

	Ensure that the relevant driver record is selected.
	Ensure the correct driver surname shows on the Delete button.
	Set the driver record as non-active. (NO shows on the Active  button).
	Click the Delete button.
You will be asked to confirm your action, once confirmed the driver record is immediately deleted from the database. However all refuelling transactions for that driver remain intact and can be reported on.

For direct polling systems the change is immediately effective however the deleted driver will still be able to refuel at remote sites until the new driver file is uploaded.

7.4 Change driver identifier number.

Should a driver identifier be lost, stolen or in any way made unusable it will be necessary to replace it and also ensure that an unauthorized person cannot use it.
This is easily achieved by issuing a new identifier and changing the related identifier in FuelManager.

You should ensure that there are no live transactions relating to the old identifier at any of your sites by initiating a communications Receive session. Any live transactions for the old identifier brought in after a change of Identifier number will not be posted but dealt with as Rejected Transactions.

	Select the driver record with the identifier to change.
	Click the Change Identifier button.
	You will be asked to confirm your action.
	Enter the new Identifier number, remembering that FuelManager will not accept duplicate numbers.

For direct polling systems the change is immediately effective, the new driver file must be uploaded to the remote sites.

7.5 Messaging.

Sending a message to be displayed when a vehicle next refuels is available for systems where direct polling is employed only.

Click the Message button to enter a message for the selected driver.
Messages can be a maximum of 24 characters long.
Normally the message is removed once it has been displayed at the refuelling point, however by ticking the Repeat Message box it will continue to appear every time the driver refuels until the message is deleted at FuelManager.

Clicking the Active Message button will open a screen showing all messages currently in use. Messages can be deleted by marking them and clicking the Delete Records button.



7.6 Find driver.

The Find Driver feature provides a quick and easy means of locating a particular driver within a large vehicle database. It can be accessed from both the Driver Registration and Driver Record screens. The search is based on all or part of the Surname and/or Personnel no.

7.7 Reports

Access to the Reports facility, which is described later in this manual.


8	Driver Record.

The Driver Record screen is accessed via the Driver Record button on the Driver Registration screen.



8.1	Password protection.

This screen shows personal and possibly sensitive information and can therefore be password protected.
The password facility must be activated by a TransFlo engineer.

When first accessed the default password is 12345, this is indicated on the form in red. The default password remains active until you enter your own unique password.

To access the Driver Record screen enter your password in the Current Password field, use the default password if indicated. Click open Driver Record button. Correct entry of the password allows immediate access to the Driver Record screen.

To change the password: first enter the current password, then your new password. Next confirm your new password and click the Change Password button.




8.2 Driver information.

The fixed data for each driver is displayed across the top of the screen, the status of the driver is shown bottom right. This information can only be changed at the Driver Registration screen.

Completion of all fields is optional.

8.3 Apply valid cost centres.

This relates to a specialist refuelling activity described later in this manual under the heading ‘Specialised Refuelling Activity’.

9	Products.

​				


The Products screen lists and allows changes to the products(fuel types) supported by FuelManager for your particular refuelling operation.

All products require a Product Name and a Product Group. A Fuel Code is also required if the remote system operates on a numeric fuel code rather than an alpha fuel name.

A Product Name can be up to characters long and should accurately describe the product. It is important to note that vehicles, tanks, and pumps can only be registered using the products listed on the Products screen.
You should also register products for which you do not have automatic refuelling facilities if they may be bought from a third party and entered into FuelManager via the Manual Transaction screen.  This will particularly apply to lubricants.

The Product Group determines whether FuelManager treats the product as a vehicle fuel or lubricant.

A Fuel Code can be any 1 or 2 digit number but it must be the same as the Fuel Code for the designated product at all remote sites.

Note: In a number of remote system certain Fuel Codes are reserved for particular applications, e.g. 9 is used to designate lube, 8 to designate a dual(auxiliary) fuel and 7 is used for L.P.G.

9.1 Add a new product.

It is recommended that new products are only added or deleted by a TransFlo engineer

Click the Add New Product button.
Select the Product Group.
Enter the new product name and fuel code.
Click anywhere in the Product List box, if your entry has been accepted it will appear in the list.

9.2 Delete a product.

FuelManager will not allow you to delete a product that is allocated to a registered vehicle, it will however allow you to delete a product that is not associated with any vehicles but does have associated tanks.

Mark the product to be deleted with a single click on the Product List.
Click the Delete Product button. You will be given a warning and if accepted the selected product will be deleted from the database.  You will also be informed if the product cannot be deleted.

10	Site Locations.

	To enable the setting up of the system storage tanks and dispensing pumps and enable communications it is necessary to first register the name of all remote refuelling sites (locations).
	The names of the locations should be chosen with care since they will be used as part of your tank and pump descriptions and also applied to automatic refuelling transactions. They are also used for the logical presentation of reports and charts.
	
	The Location name must be unique as it is used as part of the session name for communication purposes. It can be a maximum of 25 alphanumeric characters in length.


​	


10.1 Add a location.

Click the Add Location button.
Enter the new location name. 
This is the only required field; however the communication data shown in the lower half of the screen must be completed if this site has a remote refuelling facility or is under the control of direct polling.

10.2 Communication options.

There are 3 communication options, modem connect, direct connect and direct poll.

If neither the direct poll or direct connect boxes are ticked FuelManager assumes communication is via modem. Modem connection is used for PSTN modem, GSM modem and Ethernet interface connections.

The picture above shows the Site Locations screen in modem connect configuration. 

Direct connect configuration:



The Connection ID is a unique 3 alpha character code which is sent as part of the connect string to the remote site.

Direct poll configuration:



The Local pumps Enable/Disable facility enables the user to select 2 periods of time within the 24 hour period where the pumps are available for refuelling. Optionally Saturday and Sunday can be completely excluded by ticking the relevant box. Setting Start and End periods 1 or 2 to zero will cause it to be ignored.  If all times are set to zero refuelling will be available 24 hours a day.

It is recommended that a TransFlo engineer sets up all the communication facilities.

10.3 Location list.

Shows all registered locations. Double click on a location to jump directly to that record.



11	Product Storage Tanks.



The Storage Tank screen provides not only extensive information on the state of your system fuel stocks but also acts as the gateway to all other storage tank related facilities.

The tank stock and stock value information listed on the right of the screen is updated automatically as the result of refuelling transactions, dips, product deliveries and stock value adjustments. These cannot be manually altered.

Note: The Product Delivery screen is described in full in the next chapter (12).

11.1 Adding a storage tank.

Click the Add Tank button.
Select the tank location from the Location List dropdown box. If the location you require is not on the list it must first be added via the Site Locations screen.
Enter the local tank number (tank number at remote site), FuelManager allocates H.Q. reference numbers automatically.
Enter the tank Capacity in litres and the Alarm Level in litres. The Alarm Level must not exceed 10% of capacity.
Select fuel type from the product Name dropdown box.
Other fields are optional.
The new tank will be accepted by FuelManager when you attempt to move to a different record.

The Last and Next Test fields are for information recording of tank tests.

When stock falls below the figure entered in the Re-order Level field a warning reminder shows on the Main Control Panel.
As tank stock depletes and approaches the Alarm Level a warning that must be acknowledged, shows when the Main Control Panel is activated.

Detail will appear in the Attached Pumps box as you add dispensing pumps to the system.

Once a tank has been added to FuelManager it is suggested that dip is entered to avoid the Alarm Level warning. 



11.2 Deleting a storage tank.

Go to the tank record to be deleted by using the video buttons.
Click the Delete tank button. A warning will be given that requires confirmation. The tank record will them be removed from the database.

Do not delete a tank in order to enter a modified set up as FuelManager will allocate a new H.Q. reference number to the new tank which will impact on site refuelling and the ability of FuelManager to post incoming transactions.

Note: All dispensing pumps associated with the deleted tank will also be deleted.

11.3 Modify tank.

Once registered the set up information for a tank would not normally need to be altered. However should a mistake have been made during setting up the tank or the tank changed or the product changed the basic tank details can be modified by clicking the Modify Tank button.
You can change the Capacity, Alarm Level and Product details.

This feature should be used with care since it will impact on site refuelling and the handling of incoming refuelling transactions.
Before modifying the details of any tank you should ensure that all refuelling transactions relating to the original tank set up are brought into FuelManager and posted and that the associated dispensing pumps have been deleted or updated.

11.4 Entering a tank dip.

You can enter a tank dip figure to make adjustments to tank stock. It is recommended that this is done on a regular basis, say once a month, to compensate for inaccuracies in pump readings and also for audit purposes.

Select the tank that has been dipped.
Enter the new dip figure in the Last Dip field.
Enter the dip date either manually or by using the calendar feature via the action button.
Press ‘enter’ or ‘tab’ on the keyboard to confirm the date. 

​		

You will be asked if you wish to reconcile current stock to dip.

To hold the dip figure as information only without affecting the actual stock figures click the default No button, if you click the Yes button the following adjustments are made.

	Current stock is set to the new dip figure.
	Period deliveries are set to zero.
	Period usage is set to zero.
	Life deliveries are adjusted by the difference between the dip figure and the previous stock figure.
 	Stock value, both £ and €, is adjusted using the current cost per litre figure.

11.5 Attached pumps.

Once you have registered pumps, those that are attached to a particular tank will show on the list.
You can quick view of the any attached pumps by double clicking on the particular pump in the list. This feature is for information only therefore none of the Dispensing Pump screen facilities, apart from Memo, are available.

11.6 Tank list.

For large multi-site systems the Tank List provides and easy means of jumping to a particular tank record.
Double click on the required tank to move immediately to that record.

11.7 Adjusting pence/litre figure.

The p/litre figures shown for each tank are based on the current stock and the stock value entered either at the time of a fuel delivery or later if this value is not known at the time of delivery.
There will, however be instances when the p/litre figure needs to be adjusted or corrected.


​			

Select the tank whose p/litre you wish to adjust.
Click the p/litre button, the current value is shown in the change value form. Enter the new value, this must be entered in £’s. For example 95.4p/litre would be entered as 0.954; £1.05p/litre would be entered as 1.05.
Click the tick button to confirm entry. Stock values are updated immediately to reflect the change, ensure they are correct before exiting the form.
An entry is made in the Product Deliveries List to record the change.

12	Product Delivery.

	The Product Delivery screen is accessed via the Product Delivery button on the Product Storage Tank screen.

	It is important to note that most TransFlo remote site controllers allow product deliveries to be entered at the remote site. If this is done details of the delivery will be received by FuelManager during its next communication session and added to the stock of the related tank. You should therefore ensure that the delivery details are not duplicated. This is best achieved by the system administrator dictating that all deliveries are either entered locally (at the remote refuelling site) or entered via FuelManager.

​	


	If the selected tank is linked to pumps that are controlled by direct polling a warning will be given that 
refuelling will be suspended whilst the Product Delivery screen is active.

12.1 Entering a delivery.

The Location, H.Q. Tank Reference and Current Stock fields are filled automatically and cannot be manually changed. If you have selected the wrong tank click Exit and select the correct one on the Product Storage Tank screen.

Enter the Order Number relating to this delivery, The Quantity Outstanding field will be updated to show the fuel quantity outstanding on the order. If you are not using the Fuel Order Entry facility or this delivery is not covered by an order number leave blank and move straight to the Delivery field.

Enter the quantity of product received. Quantities will be accepted that are within the range of 0.1 litre to a maximum of the tank ullage.

Accept the default of the current date or change as necessary.

The delivery quantity and date are the only details that FuelManager requires, all other fields are optional. The Confirm Delivery and Cancel Delivery buttons can be used at any time.

The Delivery Value should be entered if known or later if not. This will ensure the integrity of your stock value figures. The Value can be entered in either £ or €. 

Other fields are for information only.

When you are satisfied with the detail on the form click the Confirm Delivery button, if not click the Cancel Delivery button. All fields will be reset and the Current Stock updated.

Once confirmed the product delivery quantity is posted to the related storage tank and the transaction cannot be reversed. Should an incorrect quantity be inadvertently be confirmed the required adjustment must be made using the dip facility on the Product Storage Tank screen.

When a product delivery has been completed and confirmed FuelManager makes the following adjustments to the Product Storage Tank.

Current stock is increased by the quantity of the product delivered.
Period deliveries is increased by the quantity of the product delivered.
Pence/litre (p/litre) value is adjusted to reflect the new current stock and stock value figures.

The new p/litre value will immediately be applied to all incoming refuelling transactions.

Remember that except for direct polling systems the updated tank records must be uploaded to the remote site to enable continued refuelling.

12.2 Product deliveries list.



The Product Deliveries List shows a history of deliveries, dips and p/litre value adjustments.

12.2.1 Amending a delivery value.

A delivery value will need to be amended if the value was unknown at the time of entering the delivery and either no value or an approximate value was entered.

Select the delivery entry whose value to amend by a single click on the delivery record.
Ensure that the correct record is marked.
Click the Amend Delivery Value button.
The New Delivery Value box opens.



	Select the currency of the value to be entered.
	Enter the new value and click the tick button to confirm.
Click the Exit button to close the New Delivery Value box. If you exit without clicking the tick button the new value is ignored.

When a delivery value is amended FuelManager makes the following adjustments to the Product Deliveries List and related storage tank details.

The Product Deliveries List entry is updated with the new delivery value.
The stock value, both £ and €, of the related storage tank is increased or decreased to reflect the change in delivery value.
Pence/litre (p/litre) value is adjusted to reflect the new current stock and stock value figures.

12.2.2 Delete deliveries.
​	
Select the entries to be deleted by clicking on the entry to mark it. Pressing the ‘Ctrl’ key allows a number of entries to be marked.
Click the Delete Deliveries button. 
A warning is given, if you confirm your action the selected entries are immediately deleted.

This action will only remove the selected entries from the Product Deliveries List; it does not affect the product stock or stock value of the related storage tanks.

13	Dispensing Pumps.

The Dispensing Pumps screen provides information on the status of your system fuel pumps.



Since the data relating to your fuel pumps is not critical to the data integrity of FuelManager the detail of an existing pump can be changed at any time if you have the necessary system permission. It is however important to remember that the site refuelling systems may provide transactions based on H.Q. Pump Reference.

13.1 Adding a new dispensing pump.

Click the Add Pump button.
From the dropdown Location box select the relevant remote system site.
From the dropdown Product box select the pump product and tank from which it will draw fuel.
Enter the local (site) pump number in the Pump Number field.
FuelManager allocates the H.Q. Pump Reference.

This is all the information that FuelManager requires to set up a new pump all other fields are optional.
However it is recommended that they are completed as fully as possible since they add detail to the pump reports.
The Manufacturer and Model/Type fields show in the Attached Pumps List of the Storage Tank Screen.

FuelManager updates the Totaliser field when related refuelling transactions are posted. Therefore if the Totaliser is set to start at the actual pump reading it can be used as part of your audit check.

13.2 Deleting a dispensing pump.
​	
Before deleting a pump you should ensure that it will have no impact on refuelling activity and that all transactions relating to the pump to be deleted have been downloaded from the remote site and posted in FuelManager.

Select the pump to be deleted.
Click the Delete Pump button.
A warning is given and if you confirm your action the pump is deleted immediately.

13.3 View tank.

You can view the details of the Storage Tank from which a particular pump draws its fuel by clicking the View Tank button. This feature is for information only therefore none of the Storage Tank screen facilities, apart from Memo, are available.

13.4 Throughput figures.
The Automatic Throughput figure is updated every time a transaction for the particular pump is received and post by FuelManager.
The Manual Throughput figure is updated if a Manual Transaction is recorded in FuelManager.

14	Fuel Order Entry.



	The Fuel Order Entry screen provides a convenient means of recording and tracking fuel orders placed on suppliers.

All fields, except Notes must be completed.

The Fuel Order Entry screen can also be used to hold information on orders placed for sites that do not have a refuelling system.
Either select a remote site from the dropdown Location box or directly in type the name of any site not registered in FuelManager.

The order detail entered regarding Order Number and Quantity Ordered is used during the Product Delivery procedure and is particularly useful if bulk orders covering a number of deliveries are made.

14.1 Modifying an existing order.

This opens a datasheet detailing the full information for all orders. All fields can be amended.

14.2 Deleting fuel orders.

Old fuel orders can be deleted via the Modify Orders Datasheet.

Mark the records to be deleted by clicking in the left hand header column for the selected record and then hit the Delete key on your keyboard. A number of records can be deleted at the same time by making and dragging.
​							
	Click here to mark records

You will be warned about the deletion and given a chance to change your mind.

14.3 Cancel order and New order

Cancel Order resets all fields should you make a mistake when entering the order.

New Order resets all fields ready for another entry once previous order has been confirmed.


15	Manual Transaction.

​	

	The Manual Transaction facility provides a means of recording refuelling transactions that have not been captured by the automatic refuelling process. These will be as a result of the automatic system failing to operate, the fuel product not included in the automatic set up or the product being purchased from an outside agency.

	15.1 Entering a manual transaction.

	The Clear button can be used at any time to cancel the current entry.

	Set the date of the transaction. The default is the current date, a ‘calendar’ action button is provided for convenience. If you select a future date or a date prior to the current month you will be asked to confirm the action.

	Set the time of the transaction, if known. The default is the current time.

	Open the Registration dropdown box and select the relevant vehicle from the list. FuelManager will attempt to find matching registrations if you type directly into the box.

	The Confirm Transaction and Clear buttons are now available. 

	Up until this point most data fields have been disabled. Once the vehicle has been selected the Location, Odometer and Fuel fields are enabled allowing data entry. The vehicle Fleet number, if allocated, is also shown.

	If a Driver Name is required click the Reqd box and select from the Driver dropdown box.

	Enter the Location at which the fuel was obtained. This can be either one of your remote refuelling sites selected from the dropdown list or any other name. For example a garage name and location.

	If known enter the vehicle Odometer reading at the time of refuelling, this is important in order to maintain accurate M.P.G. figures. Should you enter a figure that FuelManager cannot reconcile you will be given a warning.
The box below the Odometer field indicates the previous and/or next odometers for the vehicle, these relate to the transaction date entered.
​	
	Enter the fuel amount purchased in the Fuel field, which is labelled with the main vehicle fuel, to 1/10 litre.
	Delivery amount is limited to the vehicle tank capacity if set on the Vehicle Record screen.
	
	Ensure the Currency Type is correctly selected. If fuel was drawn from one of your refuelling sites the Fuel Cost will be based on the p/litre figure for the related tank. The Fuel Cost can be changed as required.
	
	Auxiliary fuel details will only be enabled if the vehicle has an auxiliary fuel registered in the Vehicle Record screen. The Aux. Pump field is only enabled if the chosen Location  automatically controls the Aux. Product. 
	The Aux. Cost is based on the quantity of Aux. Product and its p/litre figure, if available. The Aux. Cost can be changed as required.
	
	If a quantity for both the main vehicle fuel and its auxiliary fuel are entered FuelManager generates two separate transactions.
	
	Use the Reference field to not any other information. Tick the Receipt to record if a receipt was produced for the transaction.
	
	Click the Confirm Transaction button when all data is entered and checked. FuelManager will confirm or otherwise that the transaction has been accepted

15.2 .Adjusting a vehicle odometer reading.

Although vehicle odometer readings can be adjusted using the Manual Transaction screen it is recommended that the Change Odometer button on the Vehicle Registration screen is used.

You need to only select the vehicle from the Registration dropdown box and enter the new/adjusted odometer reading.

Entering a transaction with a date before the current date will not affect the vehicles Latest Odometer or Distance Life figures.
To alter a vehicles odometer reading to one lower than the latest shown the transaction date must be the current date. However when the current date is used and an odometer reading lower than the Latest Odometer is entered a warning will be given as well an advice of the affect on the Distance Life figure.

A transaction record will be posted within FuelManager.

15.3 Adjusting a vehicles fuel figure.

Either a negative or positive figure can be entered in the Fuel field to adjust the vehicles Fuel Life figure
as shown on the Vehicle Record screen.

After selecting the vehicle from the Registration dropdown box you should enter both the fuel
adjustment figure and the current vehicle odometer.
If no Location is selected only the statistics for the vehicle will be adjusted. If a Location that is automatically controlled is selected the Storage Tank and Dispensing Pump figures will also be adjusted.



16	View Refuelling Transactions.
	Listing and interpreting the refuelling statistics of your fleet would normally be done via the various Reports available within FuelManager. However the View Refuelling Transactions screen provides a convenient means of quickly displaying a list of transactions that occurred between two selected dates.


​	

The default date selection is between the first day of the current month and the current day.

The View Refuelling Transactions screen shows a limited number of the transactions fields.


​	





16.1 Select for Excel.

Clicking the Select for Excel button displays your selected transaction range in datasheet form which allows you to mark some or all of these transactions for export to MS Excel.




Click here to mark transactions

The transactions are marked by clicking and holding the left mouse button on the first required transaction in the record select column and dragging down over the remainder required. The selected transactions are shown in reverse, e.g. white type on black background.
 If no records are marked they are all made available for export.

Click Export to Excel on the menubar at the top of the screen, an Excel spreadsheet named ‘AllTransactions.xls’ will open with the selected transaction. If this is not the first time this has been done the spreadsheet ‘AllTransactions.xls’ may already exist if the previous version was not renamed. Either overwrite the old version or rename it via ‘Windows Explorer’.

All transaction fields are exported.

When the spreadsheet is closed control returns to FuelManager, close the datasheet view by clicking the close button, top right or by the keys ‘Ctrl + F4’, you are returned to the original View Refuelling Transactions screen.

17	Import Fuel Card Transactions.

	Transactions collected via your company fuel cards in electronic form can be integrated into the FuelManager database.

	The card types that can currently be handled are listed in the Select Card Type dropdown box.

Once you have selected your card type you must enter the full path for the location of the fuel card data file.


​			


	Although fuel card transactions usually do not directly indicate the driver, if the fuel card number is registered against a driver (in the Driver Record) all relevant details of the driver will be included in the transaction.

	Whilst the data is being imported the registration and transaction number is displayed. If any transaction s cannot be posted a warning is given. These transactions can be listed via the Reports menu.

	The most common reason for non-posted transactions is that the vehicle is not registered within FuelManager. After registering or making other corrections the fuel card transactions can again be imported, any transactions already posted will not be duplicated.


18	Data Transfer.

	The facilities available via the Data Transfer screen vary depending on the communication method selected on the Locations screen and set up options set by the TransFlo commissioning engineer. These options are described in the chapter System Settings.

	Options not available will have their command buttons disabled (greyed out).

	Workstations with no communications facilities activated will only be allowed access to the Disk Transfer and View Call Log facility.





	18.1 Calling remote sites.

The remote call up facility enables connection to your refuelling sites to retrieve transactions, deliveries, etc. and send updated files, e.g. vehicle and driver files. Connection can be by direct connection or public/private telephony.

18.1.1 Set autocall times

You can select up to two times within each 24 hour period  when FuelManager will automatically initiate a call procedure to each of the sites selected in your pre-selected call plan. FuelManager will first call each site to retrieve any data available, update all necessary files and then upload all required updated files to each site.



Enter only the hour during which you want the call to be made, using the 24 hour clock, in the range 01 to 24.
Setting the hour to 00 will disable the auto call feature. FuelManager will only commence  the auto call procedure if the Main Control Panel is the active screen. 
The status of the auto call setting is displayed at the bottom of the Main Control Panel.

18.1.2 Select call list.

Determines which remote sites are included in the call plan.


All sites that have an active means of communication are included in the list. Move from the Locations Available list to the Locations Selected list to include in all subsequent call plans.
Location names are easily moved from one list to another using the buttons located between the two lists.

18.1.3 View call log.

The call log provides a full history of all calls made, with a log number and date and time stamp. For each location details of files sent and received is listed.

Records on the call log can be marked and deleted.

18.1.4 Mode selection.

Select one of three mode options from the box on the left of the Data Transfer screen to manually initiate your call plan. 

The Send Data button will initiate a call procedure that will upload all specified files to your remote sites. This should be used after changes have been made to the FuelManager database that will affect the refuelling operation.

The files that will be uploaded will have been set by the commissioning engineer to suit your operation. See section 18.2.3 below.

You can also choose to update the remote site storage tank file and/or the remote site date and time. Click on the relevant Yes button in the Update Site box. 

Should it be necessary FuelManager can be set via System Settings to update the remote site storage tank files automatically during every AutoCall session. This must be set by a TransFlo engineer and should be used with care since the site fuel stock status will mirror that in FuelManager after every call.

The Receive Current Data button will initiate a call to each selected site and retrieve all required files. The data received will automatically be integrated into the FuelManager database.

The Receive Backup Data facility enables refuelling transactions that have been backed up at a remote site to be retrieved. You can only call one site at a time, therefore if you have more than one remote site in your call plan those sites not to be called must be removed from the Locations Selected list to the Locations Available list in Select Call List.
The back up files are designated by date, you should enter the date of the file to be retrieved. For example by entering 30/06/2009 will retrieve file ‘20090630.dat’ which holds all refuelling transactions for your selected date. 
Should you inadvertently bring in repeat (duplicate) transactions these will be filtered out by FuelManager.

The Cancel button appears as soon as a communication session is initiated. This gives the user the opportunity to end the session early. Once the Cancel button is clicked FuelManager will act on it as soon as possible, e.g. if a file transfer is underway the session will not be cancelled until the current data package has been transferred and verified. Cancelling a transfer before completion will cause any partially transferred file sent to a remote site to be discarded.

The name of the Location currently connected is displayed on the Data Transfer screen as well as a progress bar giving an indication of the file transfer status.

Should a problem occur during a data transfer session a warning message will appear on the Main Control Panel.

18.2 Disk transfer.

The Disk Transfer facility allows files to be passed to and retrieved from remote site systems that have a floppy disk reader incorporated.

You will first be asked to confirm the location of the floppy disk drive (FDD), the default is drive ‘A’.
FuelManager will then check the status of the disk. If it is clean you will be asked if you want to load the export files, if not the names of the files on the disk will be checked against the files specified for download.







18.2.1 Importing transactions from disk.
​	
If Fuelmanager finds any files on the disk that it recognises as transaction or other import files the name of the file will be displayed together with the date and time generated. You will be given the opportunity to import this file. If it is a refuelling transaction file, for example ‘site.dat’ the transactions will be imported and automatically integrated into the FuelManager database.

Once a file has been successfully handled it can be deleted, however you may choose to save the disk as a back up. Remember that Fuelmanager will only load export files to a clean disk.

18.2.2 Exporting files to disk.

FuelManager will only upload files to a clean formatted disk. Once Fuelmanager has confirmed the status of the floppy disk you will be asked to confirm that you want to upload the export files.

You will first be prompted to load the System Files to disk. System Files are those required by the remote systems to verify refuelling activity, e.g. ‘vehicle.dat’,’ fuellimit.dat’ etc.  You will only need to upload these files if changes have been made to the FuelManager database since the last upload.

You will next be asked if you wish to load the Output File to disk. The Output File would typically be a file specifically designed to pass refuelling information to a fleet management, accounting or stores control software package. 
Details of the range of Output File types available are given under System Settings.

18.2.3 Transfer file options.

Depending on the operation of the site controllers at your remote refuelling sites all or some of the following files may need to be uploaded from FuelManager.

These files are listed as required in the Send File section of the System Settings screen. This will be done by your commissioning engineer.

Vehicle.dat	holds all necessary vehicle information.

Driver.dat	holds all necessary driver information.

Fuelimit.dat	holds vehicle tank capacities

Odolimit.dat	holds upper limit for odometer entry, referenced to each vehicle.

Validcc.dat	holds cost centres that individual drivers(refuellers) are authorised to refuel.

Ccentre.dat	holds cost centre data referenced to vehicle and fuel type.

Datetime.ini	holds current FuelManager date and time information.
		Generated automatically if selected in the Site Update box. Not included in the Send File list.

Tmit.dat	holds various other data, particularly tank stock information.
Generated automatically if selected in the Site Update box, or selected for automatic upload in System Settings. Not included in the Send File list.

A Control File is always uploaded, this is automatically generated. Not included in the Send File list.




18.3 Datakey options.

DataKeys are used as a means of authorising a refuelling operation. TransFlo provide two variations of DataKey systems, the PumpMaster and PumpMinder. Refer to separate specifications for each system operation.

The PumpMaster  rarely uses the DataKey option. The PumpMinder system only uses DataKeys since it has no means of data communication and all data is carried in the key memory, a DataKey is also used to transfer data between FuelManager and the PumpMinder system.

All DataKey operations require a DataKey Programmer/Reader to be connected to your PC and the relevant port number entered in System Settings. This will be done by the commissioning engineer.

Once the Programmer is switched on, to read or programme a DataKey it must inserted and turned to the right a quarter turn to the reading position.


18.3.1 PumpMaster datakey options.




The Read Key button will initiate a read sequence for both vehicle and driver DataKeys. The result of the read is displayed on the screen.

The Clear Key button clears all data from the key.

To programme a new key or change data in an existing key click Change Data. Enter the new identifier number of the key (Ident Number) and select Key Type. Note that the Key Type defaults to ‘vehicle’.
The Owner Code is set by Fuelmanager and cannot be changed.

When satisfied with the data entered click Programme Key and your entered data will be written to the key. The key can now be removed although it is suggested that a final read of the key is performed to ensure that the key is correctly programmed.




18.3.2 PumpMinder datakey options.

As mentioned above a PumpMinder system uses two key types, one for identifying the system vehicles and one for transferring data to and from FuelManager. PumpMinder  systems do not support driver recognition.
FuelManager will automatically detect the key type inserted and display the relevant screen.



The principle of reading/programming a PumpMinder Vehicle DataKey is similar to that of the PumpMaster DataKey.  
The main difference is that a PumpMinder DataKey is required to hold more data for the relevant vehicles. Input of Fuel Type, Odometer reading, Fuel Limit and Odo(meter) Limit must be completed before programming a key.




The Transfer Key is used to download parameter and blacklist data from FuelManager to the PumpMinder system and upload refuelling data from the PumpMinder system to FuelManager.
Note that the key can be loaded with either blacklist or parameter data at one time.

Should you have more than one PumpMinder system the location should be chosen from the dropdown box. 

The key is read by clicking the Read button, the key status will be displayed. If the key holds either Blacklist or Parameter data it must be cleared before it can be reused. A key loaded with refuelling transactions must have them read into FuelManager.

The Clear Key not only clears the key of data but also writes an identity string to the key so that only the location selected will accept it.

Use Load Blacklist facility to ensure that only vehicles that are Active in FuelManager can gain access to fuel. The screen will show the number of blacklisted vehicles.

The Load Parameters button allows system parameters to loaded to the key enabling the PumpMinder system to initialise correctly. You will also be asked to set up a number of timers and details of the pulser type. Do not change the system parameters without first contacting TransFlo Service.

If the key contains refuelling transactions the Input Fuel Transactions button will be enabled. You must read in the transactions by clicking this button. 

Assuming that Fuelmanager has not previously read these transactions they will be imported and integrated into the FuelManager database. However if they have been previously read and imported by FuelManager you will be given a warning together with the date and time of the previous read. If you continue the read cycle FuelManager will discard any duplicate transactions.

The key must be cleared before reuse.

18.3.3 Engineers menu.

This function is only available for the use of TransFlo engineers. It is activated via the System Settings screen, which is password controlled.

When activated an extra command button shows on the Data Transfer screen.


​	
Clicking the Engineer Menu button activates the engineer menu.
​		
​				

Ticking the Retrieve/Send Remote parameters button changes the function of the mode selection buttons on the Data Transfer screen (see 18.1.4).



	Only one remote site should be selected in the Select Call List. 

Clicking the Send Parameters button will transfer to the remote site the operating parameters for that site as entered in the FuelManager database. The parameters downloaded to the remote site include storage tank and dispensing pump information.
Once the remote site has received the full parameter file it will automatically reboot and use the parameters as sent.

Clicking the Retrieve Parameters button will bring into FuelManager the parameters of the remote site selected.

These parameters are not used by FuelManager but can be viewd by clicking on the View Remote Parameters button on the Engineers Menu. This facility is used to confirm that the remote site is correctly set up without having to visit the site. It is also used to trouble shoot any remote site problems.




19	Reports.



The Reports Menu provides in excess of 40 reports enabling you to print or just view every aspect of your fleets refuelling operation.

	To run a report, mark your selected report by clicking on it in the list and then click the Run Report button.






Depending on the Report selected you will be asked to enter and confirm the data range that the Report should cover. This will generally always include a date range.









To see a short description of the detail provided by each report, mark the report and click Brief Report Description.



20	View/Edit Rejected Transactions.

	Should a transaction be received by FuelManager that it cannot fully post it will be marked as rejected. The View/Edit Rejected Transactions button will appear on the Main Control Panel. This button only shows if rejected transactions are marked.
Fuelmanager does not partially post transactions, if the transaction cannot be fully posted it is rejected.



The Rejected Transactions list gives details of the transaction and the reason why the posting procedure failed. 

Should the reason for failure be obvious, e.g. the vehicle/driver identifier not registered; once the problem has been resolved the transaction can be reprocessed (see below). If not you should print the Rejected Transactions list via the Reports menu and contact the TransFlo service department for assistance.

Transactions can be selected and deleted as required. Once deleted, the transaction is removed from the FuelManager database and cannot be recovered.
Multiple transactions can be marked by holing the ‘Ctrl’ key whilst marking records.
20.1 Reprocess transactions.

This feature allows rejected transactions to be edited and any discrepancies to be corrected.

FuelManager will attempt to highlight the fields that it cannot resolve and therefore need correcting, but all fields should be checked for accuracy.

The picture below shows a transaction where FuelManager cannot find in its database the vehicle identifier designated in the transaction.
Once the field is edited and a known identifier entered FuelManager will complete the vehicle registration field.

When you are satisfied that the transaction detail is correct reprocessing can be attempted. The original transaction is immediately deleted and FuelManager will attempt to post the newly edited transaction. 
Should the attempt to post the new transaction fail it will be added to the Rejected Transactions list and can be re-edited.

Only one transaction at a time can be selected for reprocessing.





21	Remote Dips Received.

​	

If a dip figure for one or more storage tanks is entered at a remote site the transaction will be included in the next data transfer session and once received by FuelManager will immediately be used to adjust the stock of the relevant tank. To ensure that a correct and valid figure has been received the Remote Dips screen allows you to adjust or accept the dip figure as required.

The Remote Dips received button will only show on the Main Control Panel if there are remote dips that have not been accepted.

Full detail of each received dip is shown on this screen, the only field that can be altered is the Adjusted Dip Value. If necessary enter in this field your adjusted dip figure.

All dip records are automatically put on a Hold status. They will be held within FuelManager until either accepted or cleared.

You will be asked to confirm any Adjusted Dip Value entered.


​	

Once confirmed you should change the status of the dip entry to Accept by ticking its box.

To change your tank stocks in accordance with the dip entries you must click on the Update Tank Stocks button. All dips with an Accept status will be actioned and cleared from the screen.
If any there are any dips that have neither a Hold nor Accept status they will be deleted with no further action when you exit the Remote Dips screen.


22	Assign Remote Deliveries.



Should a fuel delivery be entered at a remote site details are transferred to FuelManager during the next communication session.

Since the amount of information that can be entered at the remote site regarding the fuel delivery is limited the opportunity to enter further information is offered by the Assign Remote Deliveries screen.

The Assign Remote Deliveries button will only show when a remote delivery is received.

Full detail of each delivery received is shown and the fields that can be edited are shown in red.

If you attempt to enter an Order Number that has not previously been entered into FuelManager you will be given the opportunity to enter it before continuing, if you decline this opportunity the Order Number will be cleared and you should enter the word ‘none’.
Deliveries will not updated and therefore cleared from this screen until either a valid number or the word ‘none’ is entered in the Order Number field.

If a delivery already has a sterling value assigned to it, that value cannot be changed here. You must go to the Product Delivery List to make any required changes.

Deliveries cannot be deleted here, again use the Product Delivery List. 

Once all changes have been made click the Exit button. If you made changes to the fuel delivery amount you will be asked to confirm your actions. An entry detailing this change in delivery amount will be added to the Product Delivery List.






23	Direct Polling.

Direct or local polling enables FuelManager to directly control and communicate with the Pump Controllers at the refuelling site local to FuelManager. This method of operation can significantly reduce the system cost and has the advantage that refuelling transactions are handled immediately. The PC on which the software is loaded must have FuelManager running all the while refuelling is required.
One site only can be designated for direct polling. FuelManager must be informed that local polling is required by ticking the relevant check box on the System Settings screen. Setting of the direct polling communications port and baud rate is done via the Site Locations screen (see 10) for the selected site.

Using the direct polling function does not restrict the site networking capability of FuelManager via modem or direct connection providing that at least a second unique communications port is available.

23.1 Direct polling controls.

The Direct Polling Controls will show on Main Control Panel.

Start Polling.	
This control initiates the polling procedure FuelManager first searches for
all pumps associated with the selected site and then checks that the communication settings are correct. If all settings are correct communication with the pump controllers commences, instructing them to ‘go on line’ allowing automatic refuelling to take place.

The Polling Data window opens to show the status of the direct polling procedure.

Stop Polling.
A warning is given advising that you are about to stop automatic refuelling at the pumps. If confirmed automatic refuelling ceases and the Polling Data window closes.

Hide Poll Window.
Hides the Polling Data window which may interfere or obstruct your view of other FuelManager screens.

Show Poll Window.
Restores the Polling Data window to full view.

When FuelManager is running on several workstations the Direct Polling Controls will show on all machines, even though only one machine is actually polling the pump controllers. This can be overcome by opening the Local Parameters screen (Shift + F4) and ticking the Do Not Show Poll Controls box.



23.2 Polling data window.


The Polling Data window shows all activity of the direct polling function. 

When a refuelling transaction is taking place the lower half of the screen shows details of the vehicle, driver (if applicable) odometer, fuel drawn etc are shown. 

Should the pumps be automatically disabled due to the settings on the Site Locations screen you are advised of the time they were disabled and re-enabled.

Any problems that may occur are also described.

The upper half of the screen shows some of the raw data being received from the controllers and this is of use to TransFlo engineers if diagnosing a problem.





24	Short Cuts.

A number of screens or functions are available via the shortcuts listed below:

Shift + F3	Show event log.

Shift + F4	Show local parameters screen.	

Shift + F5	Utilise Windows information service to send (email) data	.

Shift + F6	Activate link wizard.

Shift + F7	Show FuelManager menubar.

Shift + F8	Hide FuelManager menubar.

Shift + F9	Show maintenance screen.

Shift + F11	Show error log.

Shift + F12	Show system settings screen.

Not all of the above 	screens or functions can be accessed from every Fuelmanager screen and most need to be ‘turned on’ via the Systems Settings screen.
​	
​	
​	


25	Event Log.
​	
The Event Log can be used to provide a history of major actions that take place on a particular workstation. 

It provides details of date, time, user logon, the event object and description.







Access to the Event Log must be switched on via the Systems Settings screen.





26	Local Parameters.
​	
This screen is password protected and for TransFlo engineer use only. It can however be viewed via the Shortcut. The various functions are described below. These parameters are local to each workstation.


​	
Do not Show Poll Controls.
Hides the Direct Polling Controls on workstations that are not involved in the direct polling function.

Bar Code/Casi-Rosco Transactions.
Informs Fuelmanager that the refuelling transactions being received are in a proprietary format.

Do not Overwrite Vehicle File.
Normally when a communication session is initiated a new vehicle file is constructed by FuelManager to reflect any changes made. However if a specialist vehicle file is produced by client software this box should be ticked to ensure that FuelManager does not overwrite it.

Show Send Remote Parameters button on Comms Menu.
In some circumstances it is necessary for clients to change the link (connection) between site tanks and pumps to ensure continuity of refuelling.
This facility allows the client to make the necessary changes at FuelManager and then upload the new status to the relevant remote site.
This facility must be used with extreme care.

Disable Connect ID on Locations form.
The connect ID is used as part of the logon and verification procedure for modem or line driver type direct connect communications. However some types of interface, ethernet interface for example, have their own specialist verification procedures.

Automatically send Tank Stocks if Delivery made.
To update the tank stocks at the remote sites normally requires a toggle button to be clicked on the Data Transfer screen. In some circumstances this may be impractical so this facility ensures that stocks are updated whenever a new deliver is entered at FuelManager. 

Disable Control Panel Functions.
Ticking the various boxes will disable the relevant control button on the Main Control Panel thus limiting workstation functions.

27	Windows information service.
​	
The operation of this feature will depend on the operating platform and set up of your PC.

28	Link Wizard.

	This function is for the use of TransFlo engineers. It provides a means of easily linking the FuelManager front-end and back-end databases.

29	Maintenance Screen.

This screen gives access to the raw FuelManager records therefore great care must be exercised when using the facilities afforded.

The screen is password controlled and for the use of TransFlo engineers only.



Access to the various record sets is via clicking the appropriate button.




Full detail of each record is shown and all fields can be edited. As an example the record screen for the system storage tanks is shown below.






Use these controls to navigate through the record set.

To view the refuelling transaction records you must first select the period required, refuelling transactions are held in calendar month based record sets.

Once the period is selected you can either click Show Transactions to view the record set for the selected month or Delete Period Transactions which will removed the complete record set for the selected month from the database.



Again all fields can be edited and individual records can be deleted.
If fields are edited or transactions deleted it should be noted that related vehicle, tank and pump records are not adjusted.
30	Error Log.

Error logging within FuelManager is activated via the System Settings screen.




The log is for TransFlo engineer use and will only be set as active if problems are being experienced with the running of FuelManager.

Details are given of the error that occurred, the module in which it occurred and the error trap within that module.


31	System Settings.

Detail entered via the System Settings screen is critical to the correct operation of FuelManager. The screen is password protected and changes should only be made by a TransFlo engineer.
The screen may be viewed by accessing without entering the password.




The various data entry fields and tick boxes are described briefly below:

Session Dir
Location of the FuelManager front-end database. The default is c:\program files\fuelmanager\


Download Dir
Folder into which all incoming files are saved. Set as a sub folder of the Session Dir.

Upload Dir
Folder that holds files ready to be sent to the remote sites. Set as a sub folder of the Session Dir.

Remote Type
Specifies the system type at the remote sites and affects the way in which FuelManager operates.

Output File
The file type and layout required for any external system, e.g. fleet management or analysis software.

Owner Code
A unique customer related code, predefined by TransFlo.

Px Fuel Width
Defines resolution of fuel fields as set in remote sytem.

Server/Data Dir
Location of the FuelManager back-end database.

Activate Error Log
Causes any system errors to be written to the error log.

Activate Modem Log
Logs all modem and data transfer activity. 

Activate Odo Entry Limit
Used by direct polling sites only.
Not Selected = Reject all incorrect odometer entries.
Selected = Accept odometer if 3 entries the same.

Activate Event Log
FuelManager will log most significant events that affect database integrity.

Remote Controller Type
Not currently used.

Activate Transaction Backup
All incoming transactions are saved in raw format to sitebak.dat in the Server/Data directory.

Site Backup Available
Informs FuelManager as to whether backup transactions can be retrieved from the remote sites.

Activate Driver Details Password
Causes the Driver Record screen to be password protected.

Show Comms Engineers Button
Causes Engineers button to appear on the Data Transfer screen.

Programmer Comm Port
Select communication port number to which the DataKey Programmer is connected. Port numbers 1-20 are available.


Use Default Modem Reset
When initialising a modem the reset string designated in the modem.ini file is overwritten by the Hayes default ATZ.

Vehicle Tag Offered First
All standard direct polling FuelManager system expect a driver identifier tag (if being used) to be offered before the vehicle tag. However for some specialist operations it is necessary for the vehicle tag to be presented first.

Local Polling
Invokes the direct polling function.
Activate Communications
Allows full access to all communication functions via the Data Transfer screen.

Auto Remote Tank Update
Causes Storage Tank data to be sent to site automatically during an AutoCall communications session.

Send File ?
Files to be sent to each remote site during a communications session. Files names may be added and deleted automatically by FuelManager.

Receive File ?
Files expected to be received from the remote sites. Again FuelManager may adjust the list.

32	Output Files.

FuelManager can produce a range of file types to enable refuelling data to be easily exported to other applications, particularly fleet management systems. Exporting data to other Microsoft applications should be achieved via the menubar.
The range of file names is shown is shown in the dropdown list – Output File, on the SystemSettings screen.

Most file types listed below will produce refuelling records for both automatic and manually entered transactions. Output Files are created in the Server/data folder. The Output File can also be loaded to floppy disk or other portable memory, see Disk Transfer. Exceptions are those files specifically produced for the Ford Motor Co. which are loaded to an FMC named folder. 

The list of available file types includes FDD and all type plus FDD, e.g. csv and csv/FDD. If you require the raw refuelling transactions to be available for copying to disk, FDD must appear in the Output File name.

In general the external software that will utilise the Output File will collect and delete that file. If the file does not exist within FuelManager (after deletion) it will automatically be re-created.



32.1 Output file options.

Defuel.dat (defuel)

This file picks up both automatic and manual transactions.

dd-mm-yyhh:nnpfffffffooooooqqqq + 14 chars of location

d = day
m = month
y = year
h = hour
n = minute
p = fuel code
f = vehicle registration	7 alphanumeric characters
o = odometer		6 numeric characters
q = fuel quantity		4 numeric characters (implied 0.1 litre)

Crg / Hlwodo.dat

These files do not track the individual refuelling transactions but hold accumulated data for each registered vehicle. These files are rebuilt after each manual transaction is entered and following an automatic communications session.  The fields are comma separated. Fleet number field will adjust length to suit, other fields are fixed length.

fffffff,oooooo,qqqqqqqq

f = vehicle fleet number	7 alphanumeric characters (typically)
o = odometer		6 numeric characters
q = fuel quantity		8 numeric characters (whole litres)

Transcsv.dat csv)

A comma separated file which records each manual and automatic refuelling transaction at the time of posting. Each field may vary in length depending on the data held.

Field	1	date				dd/mm/yyyy
		2	time				hh:nn
		3	vehicle registration
		4	vehicle fleet number
		5	vehicle identifier number
		6	fuel code
		7	fuel name
		8	fuel quantity
		9	fuel cost
		10	odometer
		11	refuelling location

Transfxd.dat (fixed)

This is a fixed length file which records each manual and automatic transaction at the time of posting.

From	To	Length		
 1		10	  10		date				dd/mm/yyyy
11		15	   5		time				hh:nn
16		23	  8		vehicle registration
24		31	  8		vehicle fleet number
32		35	  4		vehicle identifier number
36		36	  1		fuel code
37		48	 12		fuel name
49		54	  6		fuel quantity
55		61	  7		fuel cost
62		68	  7		odometer
69		83	 15		refuelling location

Fbccsv.dat (fbc)

A comma separated file which records each manual and automatic transaction at the time of posting.
Each field may vary in length. The ‘account code’ is as entered in the Vehicle Record Spare1 field.
The ‘description’ field is left as a blank field, it has data injected into it from an outside source.

Field	1	vehicle cost centre
		2	account code
		3	vehicle fleet number
		4	vehicle class
		5	fuel cost
		6	fuel quantity
		7	description


Trans.dat

This is a fixed length file which records each manual and automatic transaction at the time of posting.
This file format is selected by choosing WinSVS or WinSVS/FDD from the dropdown list.

Header record
From	To	Length
  1		 8	   8		file date				ddmmyyyy
  9		12	   4		file time				hhnn
 13		18	   6		location of site
 19		57	  39		space characters
 58		58	   1		zero character
 59		91	  39		space characters
 92		92	   1		zero character

Transaction record
From	To	Length
  1		 6	   6		location of site			
  7		14	   8		transaction date			ddmmyyyy
 15		20	   6		transaction time			hhnn
 21		30	  10		vehicle registration
 31		51	  21		space characters
 52		58	   7		odometer
 59		59	   1		refuelling type			‘V’ or ‘T’
 60		69	  10		trailer registration
 70		75	   6		driver personnel number
 76		86	  11		space characters
 87		87	   1		fuel type (first character)
 88		92	   5		fuel quantity
 93		93	   1		transaction type (always ‘1’)

Refuelling type is taken from the Vehicle Record Spare1 field.

Note: The dropdown list of output files also has one named ‘tranman’, this produced a file specifically for older versions of the Tranman fleet management software and is now generally redundant.


33	Specialised Refuelling Activity.

FuelManager can deal with a number of situations where refuelling does not follow the normal pattern.

33.1 Bowser refuelling.

Cannot be used in Direct Polling mode.

A Bowser is a mobile refuelling unit , normally a mobile tanker, that is used to refuel vehicles and plant items that do not have access to a fixed refuelling point.
The Bowser refuelling facility is used to monitor fuel dispensed to and from the Bowser tank not to the Bowser tractor unit, this would be a normal refuelling function.

FuelManager can handle Bowser tanks to a maximum capacity of 100,000 litres. 
The Bowser tank will be issued with its own identifier tag which must be registered within FuelManager in the normal way, but as a Plant type. The Vehicle Registration field must start with the word BOWSER, e.g. BOWSER1. Since the Bowser is in effect a mobile tank it should also have a registered Site Location, Storage Tank and Dispensing Pump allocated within FuelManager.  The Site Location name, and therefore the tank and pump location, must be exactly the same as the vehicle registration. In the example given the Site Location would be set as BOWSER1.

When the Bowser visits a fixed refuelling point under the control of FuelManager to refill its tank the Bowser identifier is offered in the normal way but the Pump Controller will recognise that a Bowser refill has been requested. The operator will be asked to confirm the action. When confirmed the pump will be activated and refilling can commence.

Bowser refilling transactions are retrieved by FuelManager during a normal communications session. The fuel dispensed to the Bowser is handled as a normal refuelling transaction by the host pump and tank, e.g. the fuel dispensed is deducted from the host tank and added to the host pump throughput etc. However the quantity of fuel dispensed to the Bowser is additionally treated as a Fuel Delivery to the Bowser tank.

When the Bowser is used to dispense fuel to remote vehicles standard refuelling transactions are logged that relate the registered tank and pump for that Bowser.

33.2 Sales tags.

Can only be used in Direct Polling mode.

Used in situations where as well as normal driver and vehicle refuelling (using tags registered to unique drivers and vehicles), it is also necessary to refuel vehicles without registered tags, e.g. visiting vehicles which may be charged for the fuel dispensed.
Sales Tags would only be used in this circumstance where a driver tag is also presented as part of the refuelling procedure. To make the operation flow more logically at the pump controller the vehicle tag, whether it be a Sales Tag or not is presented before the driver tag.
The Sales Tags must be registered within FuelManager starting with the word SALES. When presented to the pump controller the operator will be asked to enter the vehicle registration via the alphanumeric keypad. It should be borne in mind that since FuelManager has no registration information to refer to it will accept whatever is entered as correct. Once entered the driver tag will be requested and checked, refuelling can then commence.
The vehicle registration as entered will be inserted into the refuelling transaction during posting and will be included in standard transaction reports.
The Vehicle Record for the Sales Tag will hold information of all refuelling activity totals for the tag irrespective of the registration entered.

33.3 Master tags.

Can only be used in Direct Polling mode.

Used on vehicle tag only systems where it is necessary to cater for visiting vehicles. The Master Tags must be registered within FuelManager starting with the word MASTER. Will always request an odometer entry.
When presented to the pump controller the operator will be asked to enter the vehicle registration following the same procedure as for Sales Tags.


33.4 Refueller tags.

Can only be used in Direct Polling mode.

Used on vehicle tag only systems where it is necessary to cater for visiting vehicles. The Refueller Tags must be registered within FuelManager starting with the word FUEL. 
Similar in operation to a Master Tag except that odometer will never be requested.

33.5 Cost centre based refuelling.

Cannot be used in Direct Polling mode.

This method of refuelling is used by companies undertaking vehicle servicing or PDI work also by those employing a refueller, e.g. bus and coach companies.

Vehicles are allocated to a Cost Centre which could, for example, relate to a client or particular contract. Drivers/refuellers are designated the Cost Centres that they are allowed to refuel. This feature can be used to ensure that drivers only refuel the vehicles that are allocated to them and if the Cost Centre list is kept up to date ensures that only valid Cost Centres are refuelled ensuring that where necessary the charging of refuelling is correct.

Within FuelManager drivers are registered as normal, each driver or refueller being issued with his own unique tag (identifier). It is important to enter the correct PIN for each driver as this is used to reference valid cost centre selection.
A vehicle must be registered for each fuel type that can be used within a Cost Centre e.g. if the vehicles to be refuelled under a particular Cost Centre can use either diesel or petrol, two vehicles must be registered, one for each fuel. Remember that the Vehicle Registratin field will not accept duplicates. These two vehicles would be allocated the same Cost Centre in the Vehicle Record.

Especially for PID work the tank is filled with a limited amount of fuel, say 5 or 10 litres, this should be entered in the Tank Capacity field of the Vehicle Record.




Selecting the Cost Centres that a driver is allowed to use is done via the Driver Record by clicking on the Apply Valid Cost Centres button. The Cost Centre Selection screen opens and shows the PIN and name of the selected driver. 
A list of registered Cost Centres is shown on the left. Select valid Cost Centres by clicking on each to mark it, it will be added to the Cost Centres Selected list on the right. To remove a Cost Centre from the selected list click once more on the marked Cost Centre in the Valid Cost Centres List. 
When you have finished your selection click on the Confirm Selection button.

Remember that a data communication session must be completed to transfer any changes to the remote controllers.

Note: Identifiers are not issued to individual vehicles when refuelling by Cost Centre. The refueller/driver at the remote site will be asked to enter the vehicles Cost Centre, it will be checked against their Valid Cost Centres and if correct the refuelling site controller will select the registered vehicle to which the fuel should be allocated.

Information on refuelling activity can be retrieved within FuelManager either from the Cost Centre Reports or by listing the transactions for the vehicle registered for any particular Cost Centre.

34	Backup.

Wherever possible FuelManager should be backed up automatically by your system services.

Transflo do not provide Backup software with FuelManager. Microsoft Windows offers a Backup utility that can be used, for more information search ‘Backup’ in ‘Help and Support’ via the ‘Start’ button.
You can also purchase Backup software and once installed you can easily access it via the Backup and Restore  buttons on the Exit screen ( accessed via the Exit button on the Main Control Panel).

It is recommended that the back-end database is backed up on a daily basis. 

35	Security.

	Unless your Company has specific security requirements or runs a specialised security model it is unlikely that any changes to the security set up as supplied and installed will need to be changed.

	You must have the necessary Permissions to change the system security configuration.

To access FuelManager the Default Group Accounts must exist in the active Workgroup. 

The default FuelManager Workgroup is named fuelmanagerwg.mdw and is usually located in the FuelManager install folder.

Your commissioning engineer will have ensured that the default Workgroup exists and is the active Workgroup. However should you need to join another Workgroup for other operations you must ensure that you reinstate the FuelManager default Workgroup before you attempt to run this program. 
It is possible to add the Default Group Accounts to any other Workgroup thus overcoming the necessity to change the active Workgroup. If required this must be done by your own IT personnel.

FuelManager system security provides two overlapping security models; Workgroup based security and database password security.

35.1 Database password security.

This allows you to set a single password on each workstation for FuelManager that all users must know to run the program. This must not be confused with the Logon Password. The Database Password simply allows access to the database on each workstation whereas the Logon Password together with the User Name is part of the Workgroup configuration and determines the operating permissions afforded to the user.

Whilst this is the simplest security system to implement and use it is easily compromised. All users on a workstation have the same password. 

To set a Database Password 

Close FuelManager.  If the front-end is server based ensure no other users attempt access.
Make a copy of FuelManager and store in a secure place.
Open FuelManager in ‘exclusive’ mode and on the menubar click Tools and the Security.
Select Set Database Password.
Enter your password and confirm. Click OK.

The password is now set. Each time a user tries to open the instance of FuelManager to which the password has been applied a dialogue box appears requesting the password.
Write down the password and keep in a safe place. If it is lost or forgotten you will be unable to open FuelManager and reinstallation will be necessary.

Once you have set a password the Set Database Password option changes to Unset Database Password in the Security submenu. This means that any user who knows the current password can delete or change it.

35.2 Workgroup based security.

The default FuelManager Workgroup is named fuelmanagerwg.mdw and is usually located in the FuelManager install folder. It can if required be moved to a ‘system’ folder on a server to which all workstations have network access.
If not already the active workgroup you must join fuelmanagerwg.mdw by running the Workgroup Administrator (wkgadm.exe). This is a utility usually located in the default windows system folder.
Whether you use the default Workgroup or add the Default Group Accounts to your existing workgroup you will not be able access the FuelManager program if the Default Group Accounts do not exist in the active Workgroup because certain security features have been hard coded into the FuelManager software.

Workgroup security is based on individual users and their Permissions not passwords. This allows you to set different levels of access based on the  permission they have to use the features of FuelManager.

Permission to use the various Objects (forms, reports, list etc.)  in FuelManager can be assigned either individually to each user or to the group accounts that users can join. To simplify the granting of the various permissions in FuelManager they are assigned to group accounts rather than individual users. You can then change individual users’ permissions by adding them to or removing them from the relevant group.

35.2.1 User/Group accounts.

	The system is supplied with 3 types of group account.

Admins	The highest level of permission. Permissions are automatically assigned to this account to enable system administration. There must always be at least one member of this group.

Level 0/1/2	These accounts provide the various levels of user access to the facilities of FuelManager.

Users	A built in account that all users must join.

The system is supplied with 3 default users.

admin	A built in user account that should not be used.

fmdefault	A user account set up as belonging to all group accounts enabling full access to all FuelManager facilities. This account can be used to set up other user accounts if necessary. Once other accounts have been set up and tested this account can be deleted if required.

	The default logon password for this user account is ‘12345’.

transflo	For the exclusive use of TransFlo service and commissioning engineers.

For most purposes the 3 default group accounts already set up should provide adequate flexibility.

Level0	Gives full permission to view and update data on all FuelManager screens as well as database administration rights.

Level1	Gives full permission to view and update data on all FuelManager screens without administration rights.

Level2	Gives permission to view and report only.

To add a new user or group account:

Logon to Fuelmanager using the user account fmdefault and default password 12345.
On the menubar click Tools then Security.
Select user and Group Accounts. Select the User or Group tab as required.

Click the New button, the account name box appears.
Enter the name of the new account.
Enter a Personal ID (4-20 characters).
Click OK to confirm.


The user/group name is not case sensitive but the Personal ID (PID) is case sensitive.
The account name and PID are combined to create a security identifier (SID) for each user or group account. Once you have entered a PID you can never view or change it. The exact name and PID will be needed to recreate an account that has been deleted. It is therefore recommended one person is tasked with creating new accounts and that a hard copy of account names and associated PID’s is kept safely offsite.

After you create a new user account you can add an optional case sensitive password by using the Change Logon Password tab. The password is used at logon to verify the identity of the user. 

 The User can change their own password using the Change Password button on the Main Control Panel.






35.2.2 User permissions.

There are two types of Permissions explicit and implicit. Explicit Permissions are those permissions granted directly to a user account, no other users are affected. Implicit Permissions are those permissions granted to a Group Account. Adding a user to that group grants the groups permissions to that user. 


FuelManager security iis based on implicit permissions and unless you require more flexibility than is provided by the User Groups already set there will be no need to set any further permission levels.

Permissions can be changed for a database object by members of the Admins group or by any user who has administrator permission for the relevant object.

Even though users may not currently be able to perform an action they may be able to grant themselves permission to perform the action. This is true if a user is a member of the Admins group.


​		
35.2.3 Assign or remove permissions.

The Workgroup File in use when you logged into FuelManager must contain the user and group accounts to which you want to assign Permissions. 
Click Tools on the menubar, point to Security and click User and Group Permissions. 
On the Permissions  tab select to list either Users or Groups and then click to mark the user or group whose permissions you want to assign.

Click the type of Object, report, form etc, from the Object Type dropdown box. Then click to mark the particular object from the Object Name list.

You can select multiple objects from the Object Name list by dragging through the objects you want to select or hold down the Ctrl key and click on the required objects.

Select the Permissions you want to assign or clear the permissions you want to remove for the group or user and then click  Apply. 
Repeat for additional objects or users or groups and click OK when finished.



A
Activate Driver Details Password · 53
Activate Error Log · 53
Activate Event Log · 53
Activate Modem Log · 53
Activate Odo Entry Limit · 53
Activate Transaction Backup · 53
Active · 10, 11, 12, 13, 14, 15, 16, 39
Active Message · 16
Add New Product · 19
Add Pump · 26
Adjusted Dip · 44
AllTransactions.xls · 32
Assign Remote Deliveries · 45
Attached Pumps · 21, 27
Auto Remote Tank Update · 54
B
Back-end · 5, 50, 53, 60
Backup · 3, 35, 53, 60
Blacklisting · 2, 10, 16, 39
Bowser · 3, 57, 58
Bowser · 10, 57
C
Cancel Order · 28
Change Logon Password · 62
Change Odometer · 30
Change Password · 17
Clear Key · 37, 39
Connection ID · 20
Cost Centre · 13, 58, 59, 60
Crg / Hlwodo.dat · 55
Current stock · 23, 24
D
Data Transfer · 6, 7, 33, 35, 39, 40, 50, 53, 54
Database Password · 60, 61
DataKey · 37, 38, 53
Defuel.dat (defuel) · 55
Delete · 10, 11, 19, 28, 51
Delete Deliveries · 26
Delete Records · 16
Delete tank · 22
Deleting a pump · 27
Delivery Value · 24, 25, 26
Dip · 6, 21, 22, 23, 24, 44
Direct connect · 20
Direct poll · 20
Direct polling · 6, 9, 10, 11, 15, 16, 20, 24, 25, 46, 47, 49, 53, 54, 57, 58
Dispensing pumps · 7, 19, 21, 22, 26, 40
Distance Life · 11, 30
Download Dir · 53
Driver Record · 15, 17, 33, 53, 59
Driver Registration · 17
Drivers · 7, 14, 58
E
Engineer Menu · 39, 40
Error log · 47, 52, 53
Euro · 8
Event log · 47, 48
Excel · 8, 14, 32
F
Fbccsv.dat (fbc) · 56
FDD · 35, 54, 57
Find Driver · 14, 17
Fleet · 9, 12, 29, 55
Fmdefault · 5, 61, 62
Front-end · 5, 50, 53, 60
Fuel Card · 7, 32
Fuel Code · 18
Fuel Limit · 38
Fuel Order · 7, 24, 27
Fuel Type ·See Products
G
Group Accounts · 60, 61, 62, 63
H
Hide Poll Window · 46
I
Identifier · 9, 10, 15, 16, 37, 42, 43, 54, 55, 56, 57, 59, 62
L
Latest Odometer · 30
Load Blacklist · 39
Load Parameters · 39
Local Parameters · 3, 7, 46, 47, 49
local polling · See Direct Polling
Local pumps Enable/Disable · 20
Locations · 19, 20, 21, 24, 26, 28, 29, 30, 33, 34, 35, 46, 49, 53, 57
logon · 5, 48, 49, 61, 62
M
Main Control Panel · 5, 6, 7, 21, 34, 35, 42, 44, 46, 50, 60, 62
Maintenance · 8, 47, 50
Manual Transaction · 7, 18, 27, 29, 30
Master · 10, 58
Menubar · 8, 32, 47, 54, 60, 62, 63
Modify tank · See Storage Tanks
N
New Order · 28
O
Odo Type · 9
Odometer · 11, 14, 29, 30, 38
Odometer Limit · 14
Order Number · 24, 28, 45
Output File · 36, 53, 54
Owner Code · 37, 53
P
P/litre · 23, 25, 26, 30
Password · 5, 8, 17, 60, 61
Period Transactions · 51
Permissions · 60, 61, 63
Personnel No. · 15
Plant · 7, 57
Product Deliveries List · 23, 25, 26
Product Delivery · 2, 21, 23, 24, 28, 45
Product Group · 18, 19
Product List · 19
Product Name · 18
Product Storage Tanks · See Storage Tanks
Products · 7, 9, 18, 38
Programmer Comm Port · 53
Pump Number · 26
PumpMinder · 3, 37, 38, 39
Pumps · See Dispensing Pumps
Px Fuel Width · 53
Q
Quantity Outstanding · 24
R
Read Key · 37
Receive Backup Data · 35
Receive Current Data · 35
Receive File · 54
Refresh Links · 8
Refueller Tags · 58
Refuelling Transactions · 7, 31
Registration · 9, 10, 12, 13, 15, 17, 18, 29, 30, 57
Rejected transactions · 10, 16, 42, 43
Remote Dips · 44
Remote site · 6, 7, 10, 14, 16, 18, 20, 21, 23, 25, 27, 28,  34, 35, 40, 44, 45, 49, 54, 50, 53, 54, 59
Remote Type · 53
Repeat Message · 11, 16
Reports · 8, 13, 14, 17, 31, 33, 41, 42, 60
Retrieve Parameters · 40
Retrieve/Send Remote parameters · 40
S
Sales · 10, 58
Select Call List · 35, 40
Send Data · 35
Send File · 36, 54
Send Parameters · 40
Server/Data Dir · 53
Session Dir · 53
Set Links · 8
Show Comms Engineers Button · 53
Show Poll Window · 46
Site Backup Available · 53
Site Locations · See Locations
Specialised Refuelling Activity · 10, 18
Standard M.P.G. · 14
Start Polling · 46
stock value · 21, 23, 24, 25, 26
Stop Polling · 46
Storage Tank · 7, 21, 23, 24, 26, 27, 30, 35, 40, 54, 57
Surname · 15, 17
System Files · 36
System Settings · 3, 33, 35, 36, 37, 39, 46, 47, 48, 52
T
Tank Capacity · 14, 59
Tanks · See Storage Tanks
Tools · 8, 60, 62, 63
Trans.dat · 57
Transcsv.dat csv) · 55
Transfer · 33, 35, 36, 54
Transfer Key · 39
Transfxd.dat (fixed) · 56
U
Upload Dir · 53
Use Default Modem Reset · 54
User and Group Permissions · 63
V
Vehicle Record · 6, 9, 12, 13, 14, 30, 56, 57, 58, 59
Vehicles · 7, 9, 12, 58
Video Buttons · 6
View Call Log · 33
View Refuelling Transactions · 32
W
Workgroup · 60, 61, 63
Workgroup Administrator · 61
Workshop · 10

