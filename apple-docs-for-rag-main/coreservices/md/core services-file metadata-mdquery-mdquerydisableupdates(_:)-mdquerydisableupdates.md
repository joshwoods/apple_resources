

- Core Services
- File Metadata
- MDQuery
-  MDQueryDisableUpdates(\_:) 

Function

# MDQueryDisableUpdates(\_:)

Disables updates to the query result list.

macOS 10.4+

``` source
func MDQueryDisableUpdates(_ query: MDQuery!)
```

## Parameters 

`query`  

The query.

## Discussion

This function should be called before iterating over query results that could change due to live-updates. The disabled state is a counter and disabling can be done recursively and from different threads.

## See Also

### Starting, Stopping and Pausing Queries

func MDQueryExecute(MDQuery!, CFOptionFlags) -> Bool

Run the query, and populate the query with the results.

func MDQueryStop(MDQuery!)

Stops the query from generating more results.

func MDQueryEnableUpdates(MDQuery!)

Enables updates to the query result list.

func MDQueryIsGatheringComplete(MDQuery!) -> Bool

Returns true if the first phase of a query, the initial result gathering, has finished.

