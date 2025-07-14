

- Core Services
- File Metadata
- MDQuery
-  MDQueryEnableUpdates(\_:) 

Function

# MDQueryEnableUpdates(\_:)

Enables updates to the query result list.

macOS 10.4+

``` source
func MDQueryEnableUpdates(_ query: MDQuery!)
```

## Parameters 

`query`  

The query.

## Discussion

This function should be called when finished iterating through the list of results. Live-updates to the query results will continue when all the disables have been matched by a corresponding enable.

## See Also

### Starting, Stopping and Pausing Queries

func MDQueryExecute(MDQuery!, CFOptionFlags) -> Bool

Run the query, and populate the query with the results.

func MDQueryStop(MDQuery!)

Stops the query from generating more results.

func MDQueryDisableUpdates(MDQuery!)

Disables updates to the query result list.

func MDQueryIsGatheringComplete(MDQuery!) -> Bool

Returns true if the first phase of a query, the initial result gathering, has finished.

