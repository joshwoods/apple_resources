

- Swift
- CollectionDifference
-  init(\_:) 

Initializer

# init(\_:)

Creates a new collection difference from a collection of changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init?(_ changes: Changes) where Changes : Collection, Changes.Element == CollectionDifference.Change
```

## Parameters 

`changes`  

A collection of changes that represent a transition between two states.

## Discussion

To find the difference between two collections, use the `difference(from:)` method declared on the `BidirectionalCollection` protocol.

The collection of changes passed as `changes` must meet these requirements:

- All insertion offsets are unique

- All removal offsets are unique

- All associations between insertions and removals are symmetric

Complexity

O(*n* \* log(*n*)), where *n* is the length of the parameter.

