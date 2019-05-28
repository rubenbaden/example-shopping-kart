# example-shopping-kart
client side implementation of a basic e-shop / shopping kart

*Criteria*

- Every item (SKU) in the cart needs to have a quantity between 1 and 1000.
- Every mutation to the shopping cart needs to be recorded as an "event" with a datetime (a future user story could be about writing these mutations to e.g. Google Analytics, but for now this is out of scope!).
- Must be able to return a list of items with their quantities (as a materialized view or as is).
- Must be able to add and remove items.
- Must be able to empty the entire cart in one operation.
- Must be able to change the quantity of individual items.
- Allow for discount coupons.
- We only support fixed percentage discounts (e.g. 10%), no special business rules about combinations, times of the week, minimum amount, et cetera.
- Discount codes don't expire.
- As there is no database it is acceptable to configure the available discount codes as part of the source code.
- Only one discount can be applied to the shopping cart at a time.
- Take the optional discount into account (see the user story about discounts).
- Shipping costs are out of scope.
- There is no minimum order amount.

--

*Out of scope*

- The checkout process (including payment and handling customer information like a shipping address) is out of scope.
- Internationalization is out of scope (e.g. dealing with other timezones, currencies or languages).
- There is no minimum order.
- You can assume that there is only one shopping cart and only a single user.
- There are no shipping costs.
- You can assume that there is an unlimited amount in stock of every item.
- The data layer is out of scope (i.e. you can keep all the data in-memory and don't have to persist it to a database, for example).
