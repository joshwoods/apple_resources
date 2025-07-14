

- SwiftData
- Query
-  init(\_:animation:) 

Initializer

# init(\_:animation:)

Create a query with a SwiftData fetch descriptor.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    _ descriptor: FetchDescriptor,
    animation: Animation
) where Result == [Element]
```

## Parameters 

`descriptor`  

A `SwiftData.FetchDescriptor`.

`animation`  

The animation to use for user interface changes that result from changes to the fetched results.

## See Also

### Creating a query

init(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], animation: Animation)

Create a query with a predicate, and a list of sort descriptors.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, animation: Animation)

Creates a query with a predicate, a key path to a property for sorting, and the order to sort by.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, animation: Animation)

Creates a query with a predicate, a key path to a property for sorting, and the order to sort by.

init(FetchDescriptor&lt;Element>, transaction: Transaction?)

Create a query with a SwiftData fetch descriptor.

init(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], transaction: Transaction?)

Create a query with a predicate, and a list of sort descriptors.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, transaction: Transaction?)

Create a query with a predicate, a key path to a property for sorting, and the order to sort by.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, transaction: Transaction?)

Create a query with a predicate, a key path to a property for sorting, and the order to sort by.

