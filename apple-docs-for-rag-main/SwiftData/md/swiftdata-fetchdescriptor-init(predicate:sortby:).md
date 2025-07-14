

- SwiftData
- FetchDescriptor
-  init(predicate:sortBy:) 

Initializer

# init(predicate:sortBy:)

Creates a fetch descriptor with the specified predicate that, optionally, arranges the fetched models in a particular order.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
init(
    predicate: Predicate? = nil,
    sortBy: [SortDescriptor] = []
)
```

## Parameters 

`predicate`  

The logical condition that determines whether the fetch includes a specific model in its results. The default value is `nil`.

`sortBy`  

The array of sort descriptors that tell the fetch how to order its results. The default value is an empty array.

## Discussion

If you don’t specify a predicate, any fetch using this descriptor will return all models of the associated type. If you expect the number of fetched models to be high, use fetchLimit and fetchOffset to break those results into smaller, more efficient batches.

## See Also

### Creating a fetch descriptor

struct Predicate

A logical condition used to test a set of input values for searching or filtering.

struct SortDescriptor

A serializable description of how to sort numerics and strings.

