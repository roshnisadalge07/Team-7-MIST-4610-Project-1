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

![Data_Model](https://github.com/user-attachments/assets/293bfc6f-73db-4592-9ccb-bc900f03417c)

## Data Dictionary:
![Data_Dictionary](https://github.com/user-attachments/assets/0f1cdb1d-977d-42df-adad-5756d9a8176d)

![Data_Dictionary](https://github.com/user-attachments/assets/e23fd5b3-c495-4f1c-adcb-2a2a966d7283)

![Data_Dictionary](https://github.com/user-attachments/assets/fc741b33-f114-40c6-98af-1c627e0e664f)

![Data_Dictionary](https://github.com/user-attachments/assets/d0f93fbf-baa4-4e90-b32d-530dafd4f2ff)

![Data_Dictionary](https://github.com/user-attachments/assets/3bd14b4e-b5b4-4f29-8526-033d2799f5ed)

![Data_Dictionary](https://github.com/user-attachments/assets/93a30740-4e2c-409a-8359-ef1fb4f757d3)

![Data_Dictionary](https://github.com/user-attachments/assets/6e1edc17-cd6f-43fb-9bac-dd3db7854289)

## Queries:
![Queries](https://github.com/user-attachments/assets/37204bab-ca5e-4f11-bae6-e37f3c5dca67)

1. Query 1 displays the category name and its corresponding aisle number. The results are ordered by aisle numbers in ascending order.

![query1](https://github.com/user-attachments/assets/bac27215-5d7b-4620-a779-050882364075)

Managers can identify which category belongs to each aisle and easily know where products within that category are located. This can also be helpful to employees who are responsible for restocking shelves within each aisle. 

2. Query 2 shows the product name, how many items are currently in stock of that product, and when the product needs to be restocked. 

![query2](https://github.com/user-attachments/assets/3887f31c-6658-4554-84e3-49ffa05d242b)

This allows a manager to be aware of how many items are in stock for each product and when they must restock them. They will have constant knowledge on the inventory for their store, allowing them to keep customers happy and have a high number of sales. 

3. Query 3 lists the employee’s first and last name and their total sales if they made up 15% of total sales within the grocery store. The results were ordered in descending order of total sales.

![query3](https://github.com/user-attachments/assets/789ebcb2-17da-4db6-b4ac-41991e43ef32)

This information is useful to a manager because they are able to identify the employees who are responsible for the highest amount of sales within the store. From there, managers could make decisions on promotions or pay raises for employees who fall into this category. Ordering the total sales in descending order makes it easier to see who the overall top employee is. 

4. Query 4 finds the top-selling product in each category based on the total quantity sold.

![query4](https://github.com/user-attachments/assets/da3c4fec-906a-4628-ba32-1fd68e14b3af)

This query allows manager to identify the best-selling product in each category, helping them understand which products drive the most sales and should be prioritized in marketing efforts.

5. Query 5 shows the product names that were displayed within a certain date range (09/21 - 09/25), the quantity sold, and the total revenue made from each of those products.

![query5](https://github.com/user-attachments/assets/84ad98e3-d348-4d5d-baed-5061fa23ade5)

A manager can utilize this information to identify what products generated the highest amount of revenue within a smaller period of time and can make decisions for future sales.

6. Query 6 outputs the product name of products that were sold a total of less than two times.

![query6](https://github.com/user-attachments/assets/b583f152-9b3e-4e5d-bb40-35784b32b077)

The information provided by this query can let a manager decide what products are not as popular or are not selling as well as other products within the grocery store. This can help them when they need to put in orders for new inventory and if they want to purchase the low-selling products again. This can also help managers make decisions about promotions and price cuts. 

7. Query 7 shows all brand names and the corresponding contact emails for brands that have sold a total of at least four products, ordered in descending order. 

![query7](https://github.com/user-attachments/assets/13964846-ec2d-4eb6-8684-eae34b4ee43f)

Managers have the ability to see what brands are the highest performing in the grocery store and who to contact if they want to communicate with them to place more orders with the brand. The total number of products sold are ordered from highest to lowest so managers can see the most popular brand at the top of the list. 

8. Query 8 displays the category name, the amount of revenue the category generates, and the percentage of revenue that category makes up. 

![query8](https://github.com/user-attachments/assets/36708902-deae-49e0-90d7-b3580fc34485)

By showing category revenue and its corresponding percentage, grocery store managers can identify which categories are doing the best in terms of revenue and which categories are not producing as much revenue. Managers could find which categories to work on and develop, such as ordering new products, in order to generate more revenue. Results are ordered by the amount of revenue made from highest to lowest so managers can clearly identify the top category.

9. Query 9 retrieves all products and their respective brand names. 

![query9](https://github.com/user-attachments/assets/9b29694d-db8d-4e10-b792-39e2a73f3021)

This query allows managers can get a comprehensive list of products along with their associated brand names. This information allows managers to review the current product lineup and understand which brands are most represented in the inventory.

10. Query 10 lists all sales transactions and dates with the corresponding names of the employees who processed those transactions.

![query10](https://github.com/user-attachments/assets/14ebdbc8-f3ea-4d4d-9d95-db7342f272bc)

For grocery store managers, this query is helpful in tracking which employees are handling specific transactions, making it easier to monitor sales performance, manage employee accountability, and identify transaction trends across different staff members.

## Database information:

Name of the database: ha_group7

Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: CALL TP_Q1();



