

- Core Services
- File Metadata
- MDQuery
-  MDQueryStop(\_:) 

Function

# MDQueryStop(\_:)

Stops the query from generating more results.

macOS 10.4+

``` source
func MDQueryStop(_ query: MDQuery!)
```

## Parameters 

`query`  

The query.

## Discussion

Queries may be executed only once and cannot be restarted. The query will first complete processing any unprocessed results.do. That may trigger a progress notification, so be aware of that if you are stopping a query from within your progress note handler; that is, during this function, a recursive progress and/or finished notification might occur, which might recursively call your notification handler. It is safe to call this function recursively. You would call this function to stop a query that is generating way too many results to be useful, but still want to access the results that have come in so far. If a query is stopped before the gathering phase finishes, it will not report itself as finished, nor will it send out a finished notification.

## See Also

### Starting, Stopping and Pausing Queries

func MDQueryExecute(MDQuery!, CFOptionFlags) -> Bool

Run the query, and populate the query with the results.

func MDQueryDisableUpdates(MDQuery!)

Disables updates to the query result list.

func MDQueryEnableUpdates(MDQuery!)

Enables updates to the query result list.

func MDQueryIsGatheringComplete(MDQuery!) -> Bool

Returns true if the first phase of a query, the initial result gathering, has finished.

