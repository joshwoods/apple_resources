

- Metal
- MTLBlitCommandEncoder
-  copy(from:sourceOffset:to:destinationOffset:size:) 

Instance Method

# copy(from:sourceOffset:to:destinationOffset:size:)

Encodes a command that copies data from one buffer into another.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func copy(
    from sourceBuffer: any MTLBuffer,
    sourceOffset: Int,
    to destinationBuffer: any MTLBuffer,
    destinationOffset: Int,
    size: Int
)
```

**Required**

## Parameters 

`sourceBuffer`  

A buffer the command copies data from.

`sourceOffset`  

A byte offset within `sourceBuffer` the command copies from. In macOS, `sourceOffset` needs to be a multiple of `4`, but can be any value in iOS and tvOS.

`destinationBuffer`  

The destination buffer for the copy operation.

`destinationOffset`  

A byte offset within `destinationBuffer` the command copies to. In macOS, `destinationOffset` needs to be a multiple of `4`, but can be any value in iOS and tvOS.

`size`  

The number of bytes the command copies from `sourceBuffer` to `destinationBuffer`. In macOS, `size` needs to be a multiple of `4`, but can be any value in iOS and tvOS.

## Mentioned in 

Copying Data to a Private Resource

## Discussion

You can pass the same buffer to the `sourceBuffer` and `destinationBuffer` parameters if `size` is less than the distance between `sourceOffset` and `destinationOffset`.

Important

Copying data to overlapping regions within the same buffer may result in unexpected behavior.

