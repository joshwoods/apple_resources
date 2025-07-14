

- Swift
- RangeSet
-  insert(\_:within:) 

Instance Method

# insert(\_:within:)

Inserts a range that contains only the specified index into the range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
mutating func insert(
    _ index: Bound,
    within collection: C
) -> Bool where Bound == C.Index, C : Collection
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`index`  

The index to insert into the range set. `index` must be a valid index of `collection` that isn’t the collection’s `endIndex`.

`collection`  

The collection that contains `index`.

## Return Value

`true` if the range set was modified, or `false` if the given `index` was already in the range set.

## Discussion

Complexity

O(*n*), where *n* is the number of ranges in the range set.

