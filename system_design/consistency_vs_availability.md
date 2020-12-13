# Consistency vs Availability

# Consistency

## Week consistency

After a W, R may or may not see it.
VoIP, video chat, realtime
Memcached

## Eventual Consistency - Data is replicated asynchronously.

Highly available systems.
After a W, R will eventually see it.
Email or DNS.

## Strong consistency - transaction based systems.

After W, R will see it.

file systems and RDBMSes.

[Google I/O 2009 - Transactions Across Datacenters.. - YouTube](https://www.youtube.com/watch?v=srOgpXECblk)

# Availability

## Fail-over

### Active-passive (master-slave) failover

### Active-active (master-master) failover

Potential data loss

## Replication

[Database.](https://github.com/donnemartin/system-design-primer#database)

[Master-Slave](https://github.com/donnemartin/system-design-primer#master-slave-replication)
[Master-Master](https://github.com/donnemartin/system-design-primer#master-master-replication)
