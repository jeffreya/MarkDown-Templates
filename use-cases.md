# High-Level Business Scenario + Use Case (separate for 3rd party and Corvid)

# 3rd Party Use Case
1. The reason the 3rd party wants to use this functionality (what they plan to build on top of the API).
2. The step-by-step process the user will follow to complete this scenario, including the specific endpoint/function they will use.
**Note**: You can reference [this doc](https://docs.google.com/document/d/18TDU40kPEmVxHNJ5AFNPo82DDgPv5uLIYGeOiGJFLjI/edit) for more REST examples.

\< </br>
For example: 
## Import my products to the customer’s Wix site and offer complete drop-shipping services.
1. Import products - Use Create Product Endpoint
1. Sign up for Order Created webhook
1. When an order is made - find items, prepare packing slip and shipping label 
   1. Collect [paramX, paramY, paramZ] from Webhook to call Get Order Endpoint
   1. Call Get Order Endpoint and collect  [paramX, paramY, paramZ] for product info and to populate packing slip and shipping label
1. Print packing slip and shipping label, package ordered items and ship them
1. Notify Wix when order is dispatched, including tracking data - Use Create Fulfillment Endpoint

</br>

# Corvid Use Case
## Create a custom product management page for a client, allowing them to create and update a product and insert it into a collection using the site only, without having to access the dashboard/business manager.
1. Create a form for the product details
1. Attach the createProduct() function to the form’s submit button
1. Show the user the various collections and attach the addProductsToCollection() function to each collection name
1. Show the user all the products and allow them to edit the product details with updateProductFields() function

</br> \>
