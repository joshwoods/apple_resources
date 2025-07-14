

- Core Services
- File Metadata
- MDQuery
-  MDQueryIsGatheringComplete(\_:) 

Function

# MDQueryIsGatheringComplete(\_:)

Returns true if the first phase of a query, the initial result gathering, has finished.

macOS 10.4+

``` source
func MDQueryIsGatheringComplete(_ query: MDQuery!) -> Bool
```

## Parameters 

`query`  

The query.

## Return Value

Returns `TRUE` if the first phase of a query has completed, otherwise `FALSE`.

## See Also

### Starting, Stopping and Pausing Queries

func MDQueryExecute(MDQuery!, CFOptionFlags) -> Bool

Run the query, and populate the query with the results.

func MDQueryStop(MDQuery!)

Stops the query from generating more results.

func MDQueryDisableUpdates(MDQuery!)

Disables updates to the query result list.

func MDQueryEnableUpdates(MDQuery!)

Enables updates to the query result list.

