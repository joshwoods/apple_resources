

- Swift
- UnsafeMutableRawBufferPointer
-  swapAt(\_:\_:) 

Instance Method

# swapAt(\_:\_:)

Exchanges the byte values at the specified indices in this buffer’s memory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func swapAt(
    _ i: Int,
    _ j: Int
)
```

## Parameters 

`i`  

The index of the first byte to swap.

`j`  

The index of the second byte to swap.

## Discussion

Both parameters must be valid indices of the buffer, and not equal to `endIndex`. Passing the same index as both `i` and `j` has no effect.

