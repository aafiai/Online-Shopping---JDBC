Key Functionalities

Signup Form:

A MySQL table signup stores user details (name, username, password, credit, nationality, and issuer).
The code captures user input from GUI fields (e.g., name, username, password).
After user confirmation via a pop-up dialog, it inserts the data into the signup table and notifies the user of successful signup.

Purchase Management:

Users can add items to a "cart," specifying details such as price, quantity, and total cost.
MySQL operations (INSERT INTO purchase) are used to save purchase details.
Confirmation dialogs are used to verify actions like purchases.

Cart Operations:

Buttons (e.g., Clearbtn, Updatebtn) perform specific actions:
Updatebtn: Queries the purchase table to display current cart contents and calculate the total purchase amount.
Clearbtn: Deletes all entries in the purchase table after user confirmation.
Checkout: Redirects the user to a checkout screen.

GUI Integration:

Swing Components: Uses labels, text fields, and combo boxes to capture input from users.
Dialogs: Displays confirmation prompts and error messages.

Error Handling:

Uses try-catch blocks to handle database and runtime errors, showing descriptive error messages to the user.



How It Works

User Signup:

Users provide their details via the GUI.
Data is saved in the signup table if confirmed.

Adding Items to Cart:

Users select an item, specify its price and quantity, and confirm the purchase.
The total cost is calculated and saved in the purchase table.

Viewing and Managing Purchases:

Users can view their cart, update totals, or clear all purchases.
The total cost is displayed, and the GUI updates dynamically.

Checkout:

The user finalizes their purchase and is redirected to the checkout screen.
