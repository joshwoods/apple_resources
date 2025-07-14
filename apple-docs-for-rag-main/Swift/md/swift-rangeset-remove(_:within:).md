

- Swift
- RangeSet
-  remove(\_:within:) 

Instance Method

# remove(\_:within:)

Removes the range that contains only the specified index from the range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func remove(
    _ index: Bound,
    within collection: C
) where Bound == C.Index, C : Collection
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`index`  

The index to remove from the range set. `index` must be a valid index of `collection` that isn’t the collection’s `endIndex`.

`collection`  

The collection that contains `index`.

## Discussion

Complexity

O(*n*), where *n* is the number of ranges in the range set.

