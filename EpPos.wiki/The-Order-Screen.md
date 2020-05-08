The Order screen is the main page to EpPos. It has three main parts: the Top Bar, the Product List and the Addition View.

## Top Bar
The Top Bar shows the text "EpPos" and a couple of buttons next to it. If you are using a small screen, these buttons may be hidden in a hamburger menu.

### Enter Code
The first button is the Enter Code button. This button allows you to add a product to the current Order by code. A dialog will open with the textbox already selected. It will stay open after entering a code and pressing enter, this is so you can use a barcode scanner to quickly add a lot of products.

### Clear Order
Clear Order is a dangerous button. It removes all products from the running order. Be careful!

### Payment
Payment opens a dropdown menu, allowing you to pick between paying by Card, or with Cash. When the customer pays by Cash, the amount will be added to your current Cash (e.g. the amount of money in your register). Then the system will ask you if you want to print the addition. If you say yes (may be called `OK`) it will open up a new page and open your system printing dialog.

### Reset Cash
Reset Cash will only be shown if your current user is an admin. This allows you to set the program's "Cash" amount to any amount you want, e.g. after emptying your register.

### View Stock
View Stock will only be shown if your current user is an admin. View Stock opens a new page, listing all Products on for which stock is kept and their amount. A print button in the top left allows you to print the page.

### Admin
Admin will only be shown if your current user is an admin. The Admin page is described in the First Run Wiki Page.

### Log out
Logs the current user out of the system and returns to the login screen.

## Product List
The Product List shows a large, touchscreen friendly button for each Product. The price is displayed underneath the name. Tapping a button will add it to the current Order. When a product uses the Stock feature, you cannot add more than is currently in stock. For now, this does not show a warning.

## Addition View
The Addition View shows a list of all Products currently in the Order, with their prices and a red button with an "X" to remove them from the order. The total is displayed at the bottom.