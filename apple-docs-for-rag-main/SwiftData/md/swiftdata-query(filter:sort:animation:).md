

- SwiftData
-  Query(filter:sort:animation:) 

Macro

# Query(filter:sort:animation:)

Fetches a sorted subset of the attached model type that satisfy the specified predicate.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(accessor) @attached(peer, names: prefixed(`_`))
macro Query(
    filter: Predicate? = nil,
    sort descriptors: [SortDescriptor] = [],
    animation: Animation
) where Element : PersistentModel
```

## Parameters 

`filter`  

The logical condition the query uses to determine if it returns a specific model instance.

`descriptors`  

An array of sort descriptors to use when arranging the fetched models.

`animation`  

The animation to use when updates to the fetched models trigger user interface changes.

## See Also

### Predicate-based queries

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, animation: Animation)

Fetches a subset of the attached model type, in a specific order, by sorting on a nonoptional attribute.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, animation: Animation)

Fetches a subset of the attached model type, in a specific order, by sorting on an optional attribute.

macro Query&lt;Element>(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], transaction: Transaction?)

Fetches and sorts the subset of the attached model type that satisfy the specified predicate.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, transaction: Transaction?)

Fetches a subset of the attached model type, in a specific order, by sorting on a nonoptional attribute.

macro Query&lt;Value, Element>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, transaction: Transaction?)

Fetches a subset of the attached model type, in a specific order, by sorting on an optional attribute.

