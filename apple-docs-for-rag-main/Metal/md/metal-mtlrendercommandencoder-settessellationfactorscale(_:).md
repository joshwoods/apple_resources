

- Metal
- MTLRenderCommandEncoder
-  setTessellationFactorScale(\_:) 

Instance Method

# setTessellationFactorScale(\_:)

Configures the scale factor for per-patch tessellation factors.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setTessellationFactorScale(_ scale: Float)
```

**Required**

## Parameters 

`scale`  

A positive, normal floating-point scale factor the render pass applies to the per-patch tessellation factors.

The value of `scale` can’t be negative, infinite, equal to `NaN` (not a number), or a denormalized number.

## Discussion

The command converts `scale` to a half-precision floating-point value before it applies it to the per-patch tessellation factors (see setTessellationFactorBuffer(_:offset:instanceStride:)).

## See Also

### Configuring Tessellation Factors

func setTessellationFactorBuffer((any MTLBuffer)?, offset: Int, instanceStride: Int)

Configures the per-patch tessellation factors for any subsequent patch-drawing commands.

**Required**

