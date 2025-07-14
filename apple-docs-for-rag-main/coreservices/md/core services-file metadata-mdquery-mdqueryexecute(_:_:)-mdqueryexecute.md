

- Core Services
- File Metadata
- MDQuery
-  MDQueryExecute(\_:\_:) 

Function

# MDQueryExecute(\_:\_:)

Run the query, and populate the query with the results.

macOS 10.4+

``` source
func MDQueryExecute(
    _ query: MDQuery!,
    _ optionFlags: CFOptionFlags
) -> Bool
```

## Parameters 

`query`  

The query to execute.

`optionFlags`  

A bitwise OR of the `MDQueryOptionFlags` to be used by the query.

## Return Value

Returns `TRUE` if the query was started, `FALSE` otherwise. Queries cannot be executed more than once.

## Discussion

Queries only gather results or process updates while the current thread's run loop is running.

Queries have two phases: the initial gathering phase that collects all currently matching results and a second live-update phase. Updates occur during the live-update phase if a change in a file occurs such that it no longer matches the query or if it begins to match the query. Files which begin to match the query are added to the result list, and files which no longer match the query expression are removed from the result list.

Query notifications are posted within the context of the same thread which executes the query.

## See Also

### Starting, Stopping and Pausing Queries

func MDQueryStop(MDQuery!)

Stops the query from generating more results.

func MDQueryDisableUpdates(MDQuery!)

Disables updates to the query result list.

func MDQueryEnableUpdates(MDQuery!)

Enables updates to the query result list.

func MDQueryIsGatheringComplete(MDQuery!) -> Bool

Returns true if the first phase of a query, the initial result gathering, has finished.

