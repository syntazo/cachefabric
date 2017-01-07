# CacheFabric
*the technology behind data fabric*


## What is CacheFabric ?

Free & open source, high-performance, distributed p2p memory object caching system, generic in nature, but intended for use in speeding up dynamic applications by alleviating database load, data transferload by keeping what you need local.

CacheFabric is a drop-in replacement for memcached

CacheFabric is simple yet powerful. Its simple design promotes quick deployment, ease of development, and solves many problems facing large data caches. Its API is available for most popular languages.



* Distributed Cache
* Hot/Cold Data locality control
* Arcoss Data centers
* Eventual Consistancy
* Native memory storage avoids garbage collection and provides predictable low latency across different applications without affecting each other
* Java, .NET and C++ applications can use native client libraries to access the cache. For other languages, applications can use Hazelcast REST and Memcached interfaces
* CacheFabric   lets you monitor cache server nodes, connected clients, and used caches. It will now give notification when certain cluster management operations take too long, helping to identify performance and stability issues.
* WAN Replication lets you replicate the cache across multiple data centers.
* JCache and Map Interfaces are two standard APIs provided by CacheFabric. JCache is standard for JSR 107 and Map Interface is based on java.util.Map
* MapStore and CacheStore, respectively for Map and JCache, can be used to make CacheFabric automatically load and store data from a database
* CacheFabric High Density Memory Store (HDMS) for Near Cache (behind the JCache API) allows each app server to store hundreds of GB of cached data in memory locally (as opposed to the ~3.5 GB practical limit for on-heap data).
* High Density Memory Store for Near Cache allows each app server to access data faster: in microseconds instead of milliseconds.
* Cache-as-a-service can be updated independently of the applications (for minor-version updates). Applications using cache-as-a-service don’t need to upgrade in lock-step when cache-as-a-service is patched or upgraded, making cache-as-a-service much easier to use and giving independent applications more autonomy.





