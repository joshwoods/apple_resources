

- Metal
- MTLBlitCommandEncoder
-  fill(buffer:range:value:) 

Instance Method

# fill(buffer:range:value:)

Encodes a command that fills a buffer with a constant value for each byte.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.11+tvOS 8.0+visionOS

``` source
func fill(
    buffer: any MTLBuffer,
    range: Range,
    value: UInt8
)
```

## Parameters 

`buffer`  

A buffer instance the command assigns each byte in `range` to `value`.

`range`  

A range of bytes within the `buffer` the command assigns `value` to. The range’s count property needs to be greater than `0`. The range’s count, lowerBound, and upperBound properties need to be a multiple of `4` in macOS, but can be any value in iOS and tvOS.

`value`  

The value to write to each byte.

