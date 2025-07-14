

- SwiftUI
- FetchRequest
-  init(fetchRequest:transaction:) 

Initializer

# init(fetchRequest:transaction:)

Creates a fully configured fetch request that uses the specified transaction when updating results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
init(
    fetchRequest: NSFetchRequest,
    transaction: Transaction
)
```

Available when `Result` conforms to `NSFetchRequestResult`.

## Parameters 

`fetchRequest`  

An NSFetchRequest instance that describes the search criteria for retrieving data from the persistent store.

`transaction`  

A transaction to use for user interface changes that result from changes to the fetched results.

## Discussion

Use this initializer if you need a fetch request with updates that affect the user interface based on a Transaction. Otherwise, use init(fetchRequest:animation:).

## See Also

### Creating a fully configured fetch request

init(fetchRequest: NSFetchRequest&lt;Result>, animation: Animation?)

Creates a fully configured fetch request that uses the specified animation when updating results.

