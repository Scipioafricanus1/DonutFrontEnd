An AngularJS Front-end connecting to David Harris' Back-end.

Immediate TODO's:

Add shopping cart at top right in toolbar
use localStorage to save things to shopping cart for the checkout view later.
add form component for filling CC information with routerOutlet pointing to a separate url.
add
DonutShop Schema description:

Products Table: Shows product name, price, size.

States table: StateCode and stateName. Just used for location

Addresses table: All the bits of the address in fields, references States.

Customers table: Contains Address reference, FName, LName, Email, UserType.

Store table: AddressId referenced, StoreName, TaxRate,

Orders table: orderDate, totalPrice, references storeID.

OrderDetails: productID, OrderID, CustomerID, TotalPrice, references: CustomerId, OrderId, ProductId.

Views:

Customer view: customer will input his details in a Form View along with his/her address, state.

Home view:

Has location search bar to find a location near the customer. Color design will be pastels with donut and pastry pictures representing the donut shops.
Top bar will have Home, About, Order Now, Gallery( maybe ),, Contact Us, Careers.
A centered logo for the Donut Shop Franchise. somewhere in the layout.
State of the view: when you hit the search for the location nearest you, will show a slightly different view with a list of locations based on distance.

Locations View:

shows the search bar right below the constant Top Bar.
Contains list of locations nearest customer's location with their addresses and links to their numbers.
Order View: Maybe can order online, so when the user clicks order now, they get this view.

Shows a list of products on display to user with the details of the product and maybe an image representing that picture.
Adding items by clicking on the item in the view with a separate view that prompts user to add it to checkout, possibly with more details on the specific product like Ingredients, etc.
Checkout View: Prompts user to fill out name, Notes for order, address, shows list of items in order at top Then click check out. Payment View: Prompts user to fill out payment information or pay at reception of the order. Another form for CC info.

Could Do's:

Checkmark for sending emails regarding new deals like every other site does.
Login for returning customers to make easy orders with their information already filled out.



# DonutApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.8.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
