# Comparing SQL and NoSQL For HFT Data
SQL and NoSQL are two different methods of implementing databases that are used to store datasets based on the structure of such data. SQL (such as MySQL) is a relational database that assures Atomicity, Consistency, Isolation, and Durability (ACID) principles, which are principles that enforce the reliability of data. A great use case of this would be on banking transactions, where strictness and protocol are important in ensuring transaction conditions are met and compliant. 

On the other hand, NoSQL (such as MongoDB, which is a document-type NoSQL) is a database that relaxes the ACID principles in order to optimise for big data (semi-structured and unstructured data arriving in high volume and velocity), using flexible schemas that offer some structure to these types of data. Also, NoSQL conforms to the Basically Available, Soft state, Eventually consistent (BASE) principles to ensure that data is eventually reliable as it prioritises scalability and availability. 


Therefore, great use cases of NoSQL would fall under real-time analytics of financial feed or market data, as they arrive too quickly and in such large volumes for a relational database that wants to ensure the atomicity (during a transaction, an update might fail in one side, whilst the other updates might be successful, causing a “partial transaction”), consistency (as when checking for the condition of a certain data, it might evaluate to true even if a very quick data evaluates it to false and it wasnt detected on time), and isolation (two transactions purchasing one item could occur at the same time, due to data inconsistencies) principles.


As High-Frequency Trading (HFT) relies on real-time analysis and fast order executions, speed and flexibility would be the most important criteria to focus on. Therefore, a system that can handle a lot of tick market data at fast rates, making NoSQL databases (like MongoDB) the best candidate, as a relational database would not be able to scale as efficiently.

