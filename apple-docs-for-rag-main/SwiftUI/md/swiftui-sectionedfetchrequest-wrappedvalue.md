

- SwiftUI
- SectionedFetchRequest
-  wrappedValue 

Instance Property

# wrappedValue

The fetched results of the fetch request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
var wrappedValue: SectionedFetchResults { get }
```

## Discussion

This property behaves like the wrappedValue of a FetchRequest. In particular, SwiftUI returns the value associated with this property when you use SectionedFetchRequest as a property wrapper and then access the wrapped property by name. For example, consider the following `quakes` property declaration that fetches a `Quake` type that the Loading and Displaying a Large Data Feed sample code project defines:

```
@SectionedFetchRequest(
    sectionIdentifier: \.day,
    sortDescriptors: [SortDescriptor(\.time, order: .reverse)]
)
private var quakes: SectionedFetchResults
```

You access the request’s `wrappedValue`, which contains a SectionedFetchResults instance, by referring to the `quakes` property by name. That value is a collection of sections, each of which contains a group of managed objects:

```
Text("Found \(quakes.count) days of earthquakes")
```

If you need to separate the request and the result entities, you can declare `quakes` in two steps by using the request’s `wrappedValue` to obtain the results:

```
var fetchRequest = SectionedFetchRequest(
    fetchRequest: request,
    sectionIdentifier: \.day)
var quakes: SectionedFetchedResults { fetchRequest.wrappedValue }
```

The `wrappedValue` property returns an empty array when there are no fetched results; for example, because no entities satisfy the predicate, or because the data store is empty.

## See Also

### Getting the fetched results

func update()

Updates the fetched results.

