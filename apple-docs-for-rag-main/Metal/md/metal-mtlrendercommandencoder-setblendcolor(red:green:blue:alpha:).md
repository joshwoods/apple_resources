

- Metal
- MTLRenderCommandEncoder
-  setBlendColor(red:green:blue:alpha:) 

Instance Method

# setBlendColor(red:green:blue:alpha:)

Configures each pixel component value, including alpha, for the render pipeline’s constant blend color.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setBlendColor(
    red: Float,
    green: Float,
    blue: Float,
    alpha: Float
)
```

**Required**

## Parameters 

`red`  

A value for the red component for the blend color constant.

`green`  

A value for the green component for the blend color constant.

`blue`  

A value for the blue component for the blend color constant.

`alpha`  

A value for the alpha component for the blend color constant.

## Discussion

The alpha and color values apply to all the render pass’s attachments. The `red`, `green`, and `blue` color parameters apply to the MTLBlendFactor.blendColor and MTLBlendFactor.oneMinusBlendColor blend factors.

The `alpha` parameter applies to the MTLBlendFactor.blendAlpha and MTLBlendFactor.oneMinusBlendAlpha blend factors.

The render pipeline’s default blend color value is `0.0` for each parameter, which is equivalent to MTLBlendFactor.zero. For other blending factor values, see MTLBlendFactor.

