

- SwiftUI
- FetchRequest
-  wrappedValue 

Instance Property

# wrappedValue

The fetched results of the fetch request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
var wrappedValue: FetchedResults { get }
```

## Discussion

SwiftUI returns the value associated with this property when you use FetchRequest as a property wrapper, and then access the wrapped property by name. For example, consider the following `quakes` property declaration that fetches a `Quake` type that the Loading and Displaying a Large Data Feed sample code project defines:

```
@FetchRequest(fetchRequest: request)
private var quakes: FetchedResults
```

You access the request’s `wrappedValue`, which contains a FetchedResults instance, by referring to the `quakes` property by name:

```
Text("Found \(quakes.count) earthquakes")
```

If you need to separate the request and the result entities, you can declare `quakes` in two steps by using the request’s `wrappedValue` to obtain the results:

```
var fetchRequest = FetchRequest(fetchRequest: request)
var quakes: FetchedResults { fetchRequest.wrappedValue }
```

The `wrappedValue` property returns an empty array when there are no fetched results — for example, because no entities satisfy the predicate, or because the data store is empty.

## See Also

### Getting the fetched results

func update()

Updates the fetched results.

