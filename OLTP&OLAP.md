https://www.stitchdata.com/resources/oltp-vs-olap/

### **OLTP**

Online Transactional Processing
: A category of data processing that is focused on transaction-oriented tasks.

- captures, stores, and processes data from transactions in real time.
- typically involves inserting, updating, and/or deleting small amounts of data in a databse.
- mainly deals with large numbers of transactions by a large number of users.
- emphasis is on the **fast processing** since OLTP databases are read, written, and updated frequently.

### **OLAP**

Online Analytical Processing
: uses complex queries to analyze aggregated historical data from OLTP systems.

- emphasis is on the **response time** to complex queries. Each query involves one or more columns of data aggregated from many rows.

|                    | OLTP                                                         | OLAP                                                                       |
| ------------------ | ------------------------------------------------------------ | -------------------------------------------------------------------------- |
| Characteristics    | Handles a large number of small transactions                 | Handles large volumes of data with complex queries                         |
| Query Types        | Simple standardized queries                                  | Complex queries                                                            |
| Operations         | Based on INSERT, UPDATE, DELETE commands                     | Based on SELECT commands to aggregate data for reporting                   |
| Response Time      | Milliseconds                                                 | Seconds, minutes, or hours depending on the amount of data to process      |
| Design             | Industry-specific, such as retail, manufacturing, or banking | Subject-specific, such as sales, inventory, or marketing                   |
| Source             | Transactions                                                 | Aggregated data from transactions                                          |
| Purpose            | Control and run essential business operations in real time   | Plan, solve problems, support decisions, discover hidden insights          |
| Data Updates       | Short, fast updates initiated by user                        | Data periodically refreshed with scheduled, long-running batch jobs        |
| Space Requirements | Generally small if historical data is archived               | Generally large due to aggregating large datasets                          |
| Productivity       | Increases productivity of end users                          | Increases productivity of business managers, data analysts, and executives |
| Data View          | Lists day-to-day business transactions                       | Multi-dimensional view of enterprise data                                  |
| User Examples      | Customer-facing personnel, clerks, online shoppers           | Knowledge workers such as data analysts, business analysts, and executives |
| Database Design    | Normalized databases for efficiency                          | Denormalized databases for analysis                                        |
