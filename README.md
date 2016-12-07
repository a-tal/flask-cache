Flask-Cache

Adds easy cache support to Flask.

---

This fork of Flask-Cache includes the ability to cache with [Apache Cassandra](http://cassandra.apache.org) by setting `CACHE_TYPE`: `cassandra`.

The following config keys are available:

* `CACHE_CASSANDRA_NODES`: list of Cassandra IPs or hostnames (default: ["localhost"])

* `CACHE_CASSANDRA_PORT`: integer port number to connect on for all nodes (default: 9042)

* `CACHE_CASSANDRA_TABLE`: string table name to use in Cassandra (default: "flask_cache")

* `CACHE_CASSANDRA_KEYSPACE`: string keyspace to use in Cassandra (default: "flask_cache")

* `CACHE_CASSANDRA_REPLICATION_FACTOR`: integer [replication factor](https://cassandra.apache.org/doc/latest/architecture/dynamo.html#replication-strategy) to use (default: 1)

* `CACHE_CASSANDRA_READ_CONSISTENCY`: integer [ConsistencyLevel](https://datastax.github.io/python-driver/api/cassandra.html#cassandra.ConsistencyLevel) to use for reads (default: 1)

* `CACHE_CASSANDRA_WRITE_CONSISTENCY`: integer [ConsistencyLevel](https://datastax.github.io/python-driver/api/cassandra.html#cassandra.ConsistencyLevel) to use for writes (default: 0)

* `CACHE_CASSANDRA_DELETE_CONSISTENCY`: integer [ConsistencyLevel](https://datastax.github.io/python-driver/api/cassandra.html#cassandra.ConsistencyLevel) to use for deletes (default: 0)

* `CACHE_CASSANDRA_TABLE_CONSISTENCY`: integer [ConsistencyLevel](https://datastax.github.io/python-driver/api/cassandra.html#cassandra.ConsistencyLevel) to use for table modifications (default: 6)
