

- SwiftUI
- FetchRequest
-  init(fetchRequest:animation:) 

Initializer

# init(fetchRequest:animation:)

Creates a fully configured fetch request that uses the specified animation when updating results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
init(
    fetchRequest: NSFetchRequest,
    animation: Animation? = nil
)
```

Available when `Result` conforms to `NSFetchRequestResult`.

## Parameters 

`fetchRequest`  

An NSFetchRequest instance that describes the search criteria for retrieving data from the persistent store.

`animation`  

The animation to use for user interface changes that result from changes to the fetched results.

## Discussion

Use this initializer when you want to configure a fetch request with more than a predicate and sort descriptors. For example, you can vend a request from a `Quake` managed object that the Loading and Displaying a Large Data Feed sample code project defines to store earthquake data. Limit the number of results to `1000` by setting a fetchLimit for the request:

```
extension Quake {
    var request: NSFetchRequest {
        let request = NSFetchRequest(entityName: "Quake")
        request.sortDescriptors = [
            NSSortDescriptor(
                keyPath: \Quake.time,
                ascending: true)]
        request.fetchLimit = 1000
        return request
    }
}
```

Use the request to define a FetchedResults property:

```
@FetchRequest(fetchRequest: Quake.request)
private var quakes: FetchedResults
```

If you only need to configure the request’s predicate and sort descriptors, use init(sortDescriptors:predicate:animation:) instead. If you need to specify a Transaction rather than an optional Animation, use init(fetchRequest:transaction:).

## See Also

### Creating a fully configured fetch request

init(fetchRequest: NSFetchRequest&lt;Result>, transaction: Transaction)

Creates a fully configured fetch request that uses the specified transaction when updating results.

