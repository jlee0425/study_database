**Atomicity**: Transactions are often composed of multiple statements. Atomicity guarantees that each transaction is treated as a single "unit", which either succeeds completely, or fails completely.
If any of the statements constituting a transaction fails to complete, the entire transaction fails and the database is left unchanged.

- An atomic database must ensure atomicity in each and every situation, including power failures, errors and crashes.

**Consistency**
: Consistency ensures that a transaction can only bring the database from one _valid_ state to another, maintaining database invariants(unchanged).

- any data written to the database must be valid according to all defined rules, including constraints, cascades, triggers, and any combination thereof.
- This prevents database corruption by an illegal transaction, but **does not guarantee that a transaction is correct**.

**Isolation**
: Transactions are often executed concurrently; isolation ensures that concurrent execution of transactions leaves the database in the same state that would have been obtained if the transactions were executed sequentially.

- Isolation is the **main goal** of concurrency control.
- dependingn on the method used, the effects of an incomplete transaction might not even be visible to other transactions.

**Durability**
: Durability guarantees that once a transaction has been committed, it will remain committed even in the case of a system failure(e.g., power outage or crash).

- Usually means that completed transactions(or their effects) are recorded in non-volatile memory.
