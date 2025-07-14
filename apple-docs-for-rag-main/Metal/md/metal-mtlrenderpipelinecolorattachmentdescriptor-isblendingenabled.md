

- Metal
- MTLRenderPipelineColorAttachmentDescriptor
-  isBlendingEnabled 

Instance Property

# isBlendingEnabled

A Boolean value that determines whether blending is enabled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var isBlendingEnabled: Bool { get set }
```

## Discussion

The default value is false, meaning blending is disabled and pixel values are unaffected by blending. Disabled blending is effectively the same as the `MTLBlendOperationAdd` blend operation with a source blend factor of `1.0` and a destination blend factor of `0.0` for both RGB and alpha.

If the value is true, blending is enabled and the blend descriptor property values are used to determine how source and destination color values are combined.

## See Also

### Controlling the Blend Operation

var alphaBlendOperation: MTLBlendOperation

The blend operation assigned for the alpha data.

var rgbBlendOperation: MTLBlendOperation

The blend operation assigned for the RGB data.

