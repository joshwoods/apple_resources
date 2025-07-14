

- SwiftUI
- SectionedFetchRequest
-  init(fetchRequest:sectionIdentifier:transaction:) 

Initializer

# init(fetchRequest:sectionIdentifier:transaction:)

Creates a fully configured sectioned fetch request that uses the specified transaction when updating results.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
init(
    fetchRequest: NSFetchRequest,
    sectionIdentifier: KeyPath,
    transaction: Transaction
)
```

Available when `SectionIdentifier` conforms to `Hashable` and `Result` conforms to `NSFetchRequestResult`.

## Parameters 

`fetchRequest`  

An NSFetchRequest instance that describes the search criteria for retrieving data from the persistent store.

`sectionIdentifier`  

A key path that SwiftUI applies to the `Result` type to get an object’s section identifier.

`transaction`  

A transaction to use for user interface changes that result from changes to the fetched results.

## Discussion

Use this initializer if you need a fetch request with updates that affect the user interface based on a Transaction. Otherwise, use init(fetchRequest:sectionIdentifier:animation:).

## See Also

### Creating a fully configured fetch request

init(fetchRequest: NSFetchRequest&lt;Result>, sectionIdentifier: KeyPath&lt;Result, SectionIdentifier>, animation: Animation?)

Creates a fully configured sectioned fetch request that uses the specified animation when updating results.

