# QA-Knowledge-Check-1
Test Plan for the Shopping Cart feature for eBay

eBay has a newly implemented shopping cart that improves customer's shopping business. This new feature requires testing that covers the functions of adding/removing features work. They also have implemented a shopping cart icon that should show how many items are currently on hold before processed to checkout.

The website I have chosen for this www.ebay.com .

|Test Case # | Description | Steps | Verifying Result | Actual Result | 
|------|--------------------------------------|-----------------------------------------------|----------------------|-----------------------|-------------------------|------
 
|TSC1| Add single product to cart |User selects the product; User then clicks "Add to cart" button to add the product to cart| verify that the cart page shows the necessary links and information prior to proceeding | the product should be successfully added to the cart in the cart icon as the number 1 should be displayed|


|TSC2| Multiple products in cart| User selects product(s); click "add to cart" for item 1; choose second item and click "add to cart"| verify that the correct page shown with necessary links and informatnon before proceeeding; verify that both items are successfully added to cart; verify that the cart icon with the number 2 is displayed| the shopping cart should have both products and the cart icon displays a 2|

|TSC3| Edit item quantity from the cart| user selects product; click "add to cart" for item 1; click 'add to cart' for item 2; edit quantity of item number with valid or invalid quantities (negative, 0, with spaces)| verify that the cart page displays with all necessary links and info; verify that the product should be added to cart successfully; verify the quantity of items should br editable if user inputs an integer value; if invalid, then a warning message should display to user| User gets warning message|

|TSC4| Quantity boundaries while editing in cart | select product; click 'add to cart' for chosen product; edit quantity of item with a value greater than 5 and click checkout| verify that the following page shown with vital links and information; products should be successfully added to cart; check if item quantity number is higher than 5 then checkout is not allowed| warning error message should display to user|

|TSC5| Removing product from the cart| select product; click add to cart; click cart icon; then click on the remove product icon from the cart| product should successfully added to cart, cart icon should show 1 item; product on cart should be displayed; when product on cart is removed, then the cart should be empty and the cart icon shows 0 items| cart has no items and its icon displays "0"|

|TSC6| Removing multiple items in cart| select product(s); select add to cart for item 1; select add to cart for item 2; select the remove item from cart to remove any items from the cart | check to see if the first item is added to cart, as the cart icon should have a 1 besides it; if the second item is added to cart, check to see if the cart icon has both items and the cart icon has a 2 besides it; when removing one item from the cart, the cart should only show one item on the icon | the cart has one item and the icon has "1" |


|TSC7| Guest checkout from shopping cart| go to web app page, but do not sign in; select product, click "add to cart" and then "proceed to purchase"; go to checkout with payment/shipping options | check that the page is launched, while the page says "Hello, guest" on top of the page; check that the following pdp page shows the payment and shipping options to the user; the page then should show the user the option to sign in or continue as guest; the user should then successfully go to the checkout page with the product| user goes to checkout as a Guest|


|TSC8| Checkout from shopping cart with registered account| go to eBay and sign in with registered account; select product, click "add to cart" and then "proceed to purchase"; then it should go to checkout with payment/shipping options| check that the page is fully launched and it should display "Hello, USERNAME" on the top of the page; check that the pdp page shows payment/shipping options to the user; user should then successfully go to the checkout page with product| User proceeds to checkout with an account|

|TSC9| - applying one time discount coupon
- select product and add it to cart
- and use corresponding discount coupon in specified field while in the checkout

- check to see if the coupon applied should deduct the product price correctly

|TSC10| - duplicate discount coupon codes
- select product and add to cart
- apply the same discount coupon code (used from the same product earlier) while in checkout

- check to see if an error message pops up that states "This coupon has already been apploed."
