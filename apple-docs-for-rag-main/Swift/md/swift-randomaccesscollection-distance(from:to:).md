

- Swift
- RandomAccessCollection
-  distance(from:to:) 

Instance Method

# distance(from:to:)

Returns the distance between two indices.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func distance(
    from start: Self.Index,
    to end: Self.Index
) -> Int
```

**Required** Default implementation provided.

## Parameters 

`start`  

A valid index of the collection.

`end`  

Another valid index of the collection. If `end` is equal to `start`, the result is zero.

## Return Value

The distance between `start` and `end`. The result can be negative only if the collection conforms to the `BidirectionalCollection` protocol.

## Discussion

Unless the collection conforms to the `BidirectionalCollection` protocol, `start` must be less than or equal to `end`.

Complexity

O(1)

## Default Implementations

### BidirectionalCollection Implementations

func distance(from: Self.Index, to: Self.Index) -> Self.Index.Stride

Returns the distance between two indices.

