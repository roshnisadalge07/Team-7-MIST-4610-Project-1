# Team-7-MIST-4610-Project-1

## Team Name: 
39217 Group 7

## Team Members:

1. Chen, Jennie [@JennieC044](https://github.com/JennieC044)
2. Ferington, Nick [@NickFer5](https://github.com/NickFer5)
3. Lawler, Elena [@eglawler03](https://github.com/eglawler03)
4. Pham, Shawn [@ShawnPham21](https://github.com/ShawnPham21)
5. Sadalge, Roshni [@roshnisadalge07](https://github.com/roshnisadalge07)

## Problem Description:
Our Grocery Store Database depicts a database system to streamline the operations of a Grocery Store business. This database facilitates the management of key functions such as inventory control, sales tracking, products and brands, and employee management. Within this centralized data system, out database enhances operational efficiency, improves data accuracy, and provide valuable insights for informed decision-making for Grocery Store Management. Ultimately, the Grocery Store Database supports the store's goal of delivering an exceptional shopping experience while optimizing resources and maximizing profitability.

## Data Model:

This data model showcases a grocery store's operational data, including products, inventory, sales transactions, and employee details. The Product entity is linked to both Category and Brand, allowing for the organization of products by type (e.g., dairy, beverages) and tracking of the brand of the products. The Inventory entity tracks product stock levels, restock quantities, and dates, ensuring that the store remains well-supplied. Sales data is captured through two interconnected tables: Sales Transaction, which logs overall transaction details like payment type and total price, and Sales Transaction Details, which records the specific products and quantity sold in each transaction. Lastly, the Employee entity connects staff members to the sales they process, supporting workforce management and performance tracking. The relationships between these entities ensure comprehensive data storage for managing day-to-day operations.

The Product entity serves as the foundation of the data model. It stores the product name, description, price, and expiration date. Category and Brand use the Product entity as the linking entity in a many-to-many relationship. A brand can be associated with many categories and a category can be associated with many brands. 

The Inventory entity has a one-to-one relationship with Product because this entity is used to simply connect the inventory information to each product.

When it comes to the Sales Transaction entity, this is connected to the Product entity through a one-to-many relationship. A product can be included in many sales transaction details, but when it comes to the specific sale transaction, each detail must be associated with one product. The Sales Transaction relates directly to the transaction details.

Finally, Employee has a one-to-many relationship with the Sales Transaction entity. Employees could have worked at plenty of sales transactions, but a sales transaction can only have one employee. The Employee entity and its relationships are used to track which employees are working which sales, allowing the grocery store to have input on its employees.

![dataModel](https://github.com/user-attachments/assets/612660cf-c879-4b86-89f4-a59821bb550e)

## Data Dictionary:
![category](https://github.com/user-attachments/assets/a56f03d2-cd08-43a5-ba01-fa076962b1b1)

![brand](https://github.com/user-attachments/assets/fe4cf581-64b2-465d-8498-6ea70419e194)

![product](https://github.com/user-attachments/assets/2e56699c-9e61-4660-97f0-8074b2c9c2d4)

![inventory](https://github.com/user-attachments/assets/86f2ff39-32c5-4979-962f-b61e51605dbd)

![employee](https://github.com/user-attachments/assets/9eee6886-3049-406e-b9b9-0c4598ce8679)

![salesTransaction](https://github.com/user-attachments/assets/e77de626-cb29-44c3-ab5f-9837a3db67f8)

![salesTransactionDetails](https://github.com/user-attachments/assets/97623304-c59a-4795-8e8a-1a11ebe53187)

## Queries:
![queryDescription](https://github.com/user-attachments/assets/b50feb20-cfa1-4e12-b20f-416a994473d9)

1. Query 1 displays the category name and its corresponding aisle number. The results are ordered by aisle numbers in ascending order.

![query1](https://github.com/user-attachments/assets/23320643-5250-4630-a025-135dd7b0eb7f)

Managers can identify which category belongs to each aisle and easily know where products within that category are located. This can also be helpful to employees who are responsible for restocking shelves within each aisle. 

2. Query 2 shows the product name, how many items are currently in stock of that product, and when the product needs to be restocked. 

![query2](https://github.com/user-attachments/assets/dbe7cd09-0900-458f-841e-cf595c01be1c)

This allows a manager to be aware of how many items are in stock for each product and when they must restock them. They will have constant knowledge on the inventory for their store, allowing them to keep customers happy and have a high number of sales. 

3. Query 3 lists the employee’s first and last name and their total sales if they made up 15% of total sales within the grocery store. The results were ordered in descending order of total sales.

![query3](https://github.com/user-attachments/assets/28fe5c5e-5362-4cb6-85f5-ac5abb2d2c0c)

This information is useful to a manager because they are able to identify the employees who are responsible for the highest amount of sales within the store. From there, managers could make decisions on promotions or pay raises for employees who fall into this category. Ordering the total sales in descending order makes it easier to see who the overall top employee is. 

4. Query 4 finds the top-selling product in each category based on the total quantity sold.

![query4](https://github.com/user-attachments/assets/5470d0ab-f8cd-4130-aed6-ef2013a0f779)

This query allows manager to identify the best-selling product in each category, helping them understand which products drive the most sales and should be prioritized in marketing efforts.

5. Query 5 shows the product names that were displayed within a certain date range (09/21 - 09/25), the quantity sold, and the total revenue made from each of those products.

![query5](https://github.com/user-attachments/assets/cba4529e-d474-47c7-a6ff-5a357b300b8d)

A manager can utilize this information to identify what products generated the highest amount of revenue within a smaller period of time and can make decisions for future sales.

6. Query 6 outputs the product name of products that were sold a total of less than two times.

![query6](https://github.com/user-attachments/assets/1ac12ebd-f80c-45cb-aa74-d609d9226c15)

The information provided by this query can let a manager decide what products are not as popular or are not selling as well as other products within the grocery store. This can help them when they need to put in orders for new inventory and if they want to purchase the low-selling products again. This can also help managers make decisions about promotions and price cuts. 

7. Query 7 shows all brand names and the corresponding contact emails for brands that have sold a total of at least four products, ordered in descending order. 

![query7](https://github.com/user-attachments/assets/d6baaeaa-5573-4fbf-804f-3f3b10f0b78b)

Managers have the ability to see what brands are the highest performing in the grocery store and who to contact if they want to communicate with them to place more orders with the brand. The total number of products sold are ordered from highest to lowest so managers can see the most popular brand at the top of the list. 

8. Query 8 displays the category name, the amount of revenue the category generates, and the percentage of revenue that category makes up. 

![query8](https://github.com/user-attachments/assets/afd92167-79c0-4ef0-8710-30e51480aa45)

By showing category revenue and its corresponding percentage, grocery store managers can identify which categories are doing the best in terms of revenue and which categories are not producing as much revenue. Managers could find which categories to work on and develop, such as ordering new products, in order to generate more revenue. Results are ordered by the amount of revenue made from highest to lowest so managers can clearly identify the top category.

9. Query 9 retrieves all products and their respective brand names. 

![query9](https://github.com/user-attachments/assets/9772ea84-ce1f-413b-84c2-b41ed8477b8a)

This query allows managers can get a comprehensive list of products along with their associated brand names. This information allows managers to review the current product lineup and understand which brands are most represented in the inventory.

10. Query 10 lists all sales transactions and dates with the corresponding names of the employees who processed those transactions.

![query10](https://github.com/user-attachments/assets/865b6b4d-409b-4e61-905b-9c46a68c208b)

For grocery store managers, this query is helpful in tracking which employees are handling specific transactions, making it easier to monitor sales performance, manage employee accountability, and identify transaction trends across different staff members.

## Database information:

Name of the database: ha_group7

All queries are bookmarked through stored procedures and can be called using this format: CALL TP_Qx(); where 'x' is the query number.



