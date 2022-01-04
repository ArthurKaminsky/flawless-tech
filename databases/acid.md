# Benefits Of ACID Design

In different situations we require that the data we store for our clients to be secure, reliable and ought to have the upmost performance capabilities.
I want to solely talk about ACID, what is it? Why should we incorperate it to our system? And what are the use cases for it?
ACID is an acronym of Atomicity, Consistency, Isolation and Durability.
It is a set of principles that apply to the database world to ensure reliability for data transactions.
ACID ensures that the database recovers from failed processed data that might occur during the transaction.

### Atomicy

Atomicity means that the transaction can either succeed or it can fail. 
Meaning that there couldn't be any partial processed data.
If the transaction has not been fully processed, then the whole transaction fails and there's no modification or any other manipulation in the database.

### Consistency

Consistency means that all data will be consistent. All data in the database will be binded with a strict set of rules which could be constraints, cascades, and triggers that could be applied to the database.

### Isolation

Isolation guarantees that all transactions will occur in isolation. No transaction will be affected by another transaction.
So a transaction cannot read data from another transaction that has not yet completed it's operation.

### Durability

Durability means that, once a transaction is committed, it will remain in the system even if there's a system crash immediately following the transaction.
Any changes from the transaction must be stored permanently. If the system tells the user that the transaction has succeeded, the transaction must have indeed succeeded.

ACID
ACID is an acronym of Atomicity, Consistency, Isolation and Durability. Is a set of
principles that apply to the database to ensure data transaction reliability.
ACID makes sure that the database recovers from failed processed data that might
occur during the transaction.
Atomicity
Atomicity means that the transaction can either succeed or it can fail. Meaning that
there couldn't be any partial processed data. If the transaction has not been fully
processed then the whole transaction fails and there's no modification in the database.
Consistency
Consistency means that all data will be consistent. All data in the database will be
binded with a strict set of rules which could be constraints, cascades, and triggers that
could be applied to the database.
As for my small research on your question about consistency, Idan:)
Most SQL relational databases such as MySQL abide heavily on ACID principles and
one of them includes Consistency. This means that the type of data that is added or
modified ought to be based on the rules of constraints if the operation to be successful
and then the data will be consistent for all observers of the entity. Since data is stored in
relations and doesn't have to be modified across every entity, it allows to have quicker
write operations with immediate effects.
In NoSQL the consistency in databases is much weaker than SQL databases. NoSQL
such as MongoDB uses more flexible data models in the form of collections and
documents. In NoSQL if we want to execute heavy reads of documents to increase
performance we'll only place necessary data in other documents that we'd want to
retrieve for faster read operations within the collection. However, if we need to perform
write operations, then not only do we need to change the document's fields in the
collection, but also the other documents in other collections that have a reference to the
main document. And such an operation requires more execution to see a consistent
view after the data has been added or modified.

I've read a little bit about MongoDB and as NoSQL database it is not ACID compliant,
but it does support ACID transactions when it comes to document transactions at the
document level.
Isolation
Isolation guarantees that all transactions will occur in isolation. No transaction will be
affected by another transaction. So a transaction cannot read data from another
transaction that has not yet completed it's operation.
For instance, if I'm in a batch operation of modifying my records and I'm committing my
changes, another transaction cannot read that data until the transaction that deals with
the modifications has not yet completed.
Durability
Durability means that, once a transaction is committed, it will remain in the system even
if there's a system crash immediately following the transaction. Any changes from the
transaction must be stored permanently. If the system tells the user that the transaction
has succeeded, the transaction must have indeed succeeded.