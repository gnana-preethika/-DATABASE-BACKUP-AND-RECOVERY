COMPANY: CODTECH IT SOLUTIONS

NAME: GNANA PREETHIKA A B

DOMAIN: SQL

DURATION: 4 WEEKS

MENTOR: NEELA SANTHOSH KUMAR


This task focuses on simulating a typical backup and recovery workflow using SQL for a relational database. It is designed to demonstrate how data can be safely backed up and restored in the event of accidental data loss or system failure. Although actual backup utilities like mysqldump or PostgreSQL's pg_dump are used in production environments, this simulation uses SQL queries to conceptually replicate those steps.

The process starts by creating an orders table that holds transactional data. This table includes five columns: order_id, customer_name, product, quantity, and order_date. These fields represent a simplified version of an e-commerce or retail order management system.

Once the table structure is defined, sample data is inserted into the table. The inserted records represent customer orders from individuals like Ananya, Ravi, and Meera, who have purchased items such as laptops, smartphones, and headphones. Each record contains relevant information about what was ordered, by whom, in what quantity, and on which date.

Following data insertion, the task simulates the backup step. In real-life scenarios, this would involve exporting the table data using tools like mysqldump, exporting to a .csv file, or using automated backup solutions. In this simulation, a SELECT * FROM orders; command is used to view and represent the current state of the table as if it were being backed up. This step is critical for ensuring that a copy of the data exists before any potential failure or data manipulation.

Next, the task demonstrates a failure simulation by dropping the orders table. This simulates a scenario where a database table is accidentally deleted or corrupted. Although the actual DROP TABLE command is commented out to prevent accidental execution, it shows the typical step involved in a failure or data loss situation.

After simulating the failure, the recovery process is initiated. The orders table structure is recreated to match the original schema exactly, ensuring that the restored data will fit the table structure properly. Following the recreation of the schema, the original records are reinserted into the table. These inserts mimic restoring from a backup file or a recovery dump.

Finally, a SELECT * FROM orders; query is run to verify that the data has been successfully restored. If all steps were followed correctly, the table will contain the same three original records, proving that the backup and recovery process worked effectively.

This task serves as an essential example for understanding the importance of regular database backups and the ability to restore systems quickly during emergencies. It reinforces database administration concepts such as disaster recovery planning, data durability, and operational continuity. The approach taken here is simplified for learning purposes but captures the essence of a real-world backup and recovery strategy using SQL.
OUTPUT:
![Image](https://github.com/user-attachments/assets/9bfdc92c-4f0b-4444-9710-b311481731b0)
