

- SwiftData
-  Query(filter:sort:order:transaction:) 

Macro

# Query(filter:sort:order:transaction:)

Fetches a subset of the attached model type, in a specific order, by sorting on a nonoptional attribute.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(accessor) @attached(peer, names: prefixed(`_`))
macro Query(
    filter: Predicate? = nil,
    sort keyPath: KeyPath,
    order: SortOrder = .forward,
    transaction: Transaction? = nil
) where Value : Comparable, Element : PersistentModel
```

## Parameters 

`filter`  

The logical condition the query uses to determine if it returns a specific model instance.

`keyPath`  

The keypath of the nonoptional attribute to sort by.

`order`  

The order of the sort.

`transaction`  

The transaction to use when updates to the fetched models trigger user interface changes.

## See Also

### Predicate-based queries

macro Query&lt;Element>(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], animation: Animation)

Fetches a sorted subset of the attached model type that satisfy the specified predicate.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, animation: Animation)

Fetches a subset of the attached model type, in a specific order, by sorting on a nonoptional attribute.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, animation: Animation)

Fetches a subset of the attached model type, in a specific order, by sorting on an optional attribute.

macro Query&lt;Element>(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], transaction: Transaction?)

Fetches and sorts the subset of the attached model type that satisfy the specified predicate.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, transaction: Transaction?)

Fetches a subset of the attached model type, in a specific order, by sorting on an optional attribute.

