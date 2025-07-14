

- Swift
- MutableCollection
-  swapAt(\_:\_:) 

Instance Method

# swapAt(\_:\_:)

Exchanges the values at the specified indices of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func swapAt(
    _ i: Self.Index,
    _ j: Self.Index
)
```

**Required** Default implementation provided.

## Parameters 

`i`  

The index of the first value to swap.

`j`  

The index of the second value to swap.

## Discussion

Both parameters must be valid indices of the collection and not equal to `endIndex`. Passing the same index as both `i` and `j` has no effect.

Complexity

O(1)

## Default Implementations

### MutableCollection Implementations

func swapAt(Self.Index, Self.Index)

Exchanges the values at the specified indices of the collection.

