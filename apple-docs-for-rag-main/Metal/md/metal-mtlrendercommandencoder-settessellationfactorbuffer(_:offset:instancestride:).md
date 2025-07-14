

- Metal
- MTLRenderCommandEncoder
-  setTessellationFactorBuffer(\_:offset:instanceStride:) 

Instance Method

# setTessellationFactorBuffer(\_:offset:instanceStride:)

Configures the per-patch tessellation factors for any subsequent patch-drawing commands.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setTessellationFactorBuffer(
    _ buffer: (any MTLBuffer)?,
    offset: Int,
    instanceStride: Int
)
```

**Required**

## Parameters 

`buffer`  

An MTLBuffer instance that stores the per-patch tessellation factors, which can’t be empty or `nil`.

`offset`  

The distance, in bytes, between the start of the data and the start of the buffer, which needs to be a multiple of `4`.

`instanceStride`  

The number of bytes between two instances of data in `buffer`, which needs to be a multiple of `4`.

## Discussion

Call this method before encoding patch-drawing commands.

## See Also

### Configuring Tessellation Factors

func setTessellationFactorScale(Float)

Configures the scale factor for per-patch tessellation factors.

**Required**

