# DAY1TASK
E-commerce

Entities:
Customer - People who shop on the platform
Product - Items available for sale
Order - Orders placed by customers
OrderItem - Specific products within an order

Relationships:
A Customer can place multiple Orders
An Order can contain multiple Products (through OrderItem)
A Product can be part of multiple Orders

Primary Keys:
customer_id in Customer
product_id in Product
order_id in Order
order_item_id in OrderItem

Foreign Keys:
customer_id in Order references Customer(customer_id)
order_id in OrderItem references Order(order_id)
product_id in OrderItem references Product(product_id)
