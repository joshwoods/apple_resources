

- Metal
- MTLRenderPassAttachmentDescriptor
-  resolveTexture 

Instance Property

# resolveTexture

The destination texture used when resolving multisampled texture data into single sample values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var resolveTexture: (any MTLTexture)? { get set }
```

## Mentioned in 

Setting Load and Store Actions

## Discussion

If the storeAction value is set to MTLStoreAction.multisampleResolve or MTLStoreAction.storeAndMultisampleResolve, then the resolveTexture value must point to a valid texture. Otherwise, Metal ignores this property.

## See Also

### Specifying the Texture to Resolve Multisample Data

var resolveLevel: Int

The mipmap level of the texture used for the multisample resolve action.

var resolveSlice: Int

The slice of the texture used for the multisample resolve action.

var resolveDepthPlane: Int

The depth plane of the texture used for the multisample resolve action.

