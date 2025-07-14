

- CloudKit
- CKQueryOperation
-  init(query:) 

Initializer

# init(query:)

Creates an operation that searches for records in the specified record zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
convenience init(query: CKQuery)
```

## Parameters 

`query`  

The query for the search.

## Discussion

You can use the operation that this method returns only once to perform a search, but you can reuse the query that you provide. During execution, the operation performs a new search and returns the first batch of results. If there are more results available, you must create a separate query object using the provided cursor object.

## See Also

### Creating a Query Operation

convenience init(cursor: CKQueryOperation.Cursor)

Creates an operation with additional results from a previous search.

init()

Creates an empty query operation.

