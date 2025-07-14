

- Core Services
- File Metadata
-  kMDQuerySynchronous 

Global Variable

# kMDQuerySynchronous

Specifies that a query should block during the initial gather phase. The query’s run loop will run in the default mode. If this option is not specified the query function returns immediately after starting the query asynchronously.

Mac Catalyst 13.0+macOS 10.4+

``` source
var kMDQuerySynchronous: MDQueryOptionFlags { get }
```

