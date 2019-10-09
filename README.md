# DonutFrontEnd
An AngularJS Front-end connecting to David Harris' Back-end.

Immediate TODO's: 
- create the angular project
- have a Top Bar that has all the bits required. Doesn't have to be functional yet, just for concept.
- have dummy product details displayed in card (do this with a model for Products, a service for grabbing the dummy data, a component that calls the service and displays the data in the card format.)

**NOTE:** Did all of the above already and also added a dummy httpClient service so I can test the service calls to a local database before we get the real api details to call from. Just need to commit at home or remake on my home computer if that's not possible.. 
- must think about how the main page view shows the donut product description in a clean way. 
- must switch themes to a pastel color for the donutApp as it's black and purple now which doesn't really fit I think.
- must study different angular material component types for ideas on how to layout things. currently defautling the <mat-card> but I think it could look better.


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
- Has location search bar to find a location near the customer. Color design will be pastels with donut and pastry pictures representing the donut shops. 
- Top bar will have Home, About, Order Now, Gallery( maybe ),, Contact Us, Careers.
- A centered logo for the Donut Shop Franchise. somewhere in the layout. 

State of the view: when you hit the search for the location nearest you, will show a slightly different view with a list of locations based on distance.


Locations View: 
- shows the search bar right below the constant Top Bar. 
- Contains list of locations nearest customer's location with their addresses and links to their numbers.

Order View: Maybe can order online, so when the user clicks order now, they get this view.
- Shows a list of products on display to user with the details of the product and maybe an image representing that picture.
- Adding items by clicking on the item in the view with a separate view that prompts user to add it to checkout, possibly with more details on the specific product like Ingredients, etc.

Checkout View: Prompts user to fill out name, Notes for order, address, shows list of items in order at top Then click check out.
Payment View: Prompts user to fill out payment information or pay at reception of the order. Another form for CC info. 

Could Do's: 
- Checkmark for sending emails regarding new deals like every other site does.
- Login for returning customers to make easy orders with their information already filled out.






