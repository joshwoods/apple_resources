

- Metal
- MTLRenderPipelineColorAttachmentDescriptor
-  destinationAlphaBlendFactor 

Instance Property

# destinationAlphaBlendFactor

The destination blend factor (DBF) used by the alpha blend operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var destinationAlphaBlendFactor: MTLBlendFactor { get set }
```

## Discussion

The default value is MTLBlendFactor.zero.

## See Also

### Specifying Blend Factors

var destinationRGBBlendFactor: MTLBlendFactor

The destination blend factor (DBF) used by the RGB blend operation.

var sourceAlphaBlendFactor: MTLBlendFactor

The source blend factor (SBF) used by the alpha blend operation.

var sourceRGBBlendFactor: MTLBlendFactor

The source blend factor (SBF) used by the RGB blend operation.

