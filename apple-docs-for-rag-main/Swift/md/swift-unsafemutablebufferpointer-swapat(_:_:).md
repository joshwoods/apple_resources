

- Swift
- UnsafeMutableBufferPointer
-  swapAt(\_:\_:) 

Instance Method

# swapAt(\_:\_:)

Exchanges the values at the specified indices of the buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func swapAt(
    _ i: Int,
    _ j: Int
)
```

## Parameters 

`i`  

The index of the first value to swap.

`j`  

The index of the second value to swap.

## Discussion

Both parameters must be valid indices of the buffer, and not equal to `endIndex`. Passing the same index as both `i` and `j` has no effect.

