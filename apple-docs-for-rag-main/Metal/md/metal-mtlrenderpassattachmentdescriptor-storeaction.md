

- Metal
- MTLRenderPassAttachmentDescriptor
-  storeAction 

Instance Property

# storeAction

The action performed by this attachment at the end of a rendering pass for a render command encoder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var storeAction: MTLStoreAction { get set }
```

## Mentioned in 

Storing Data a Pass Makes with Custom Sample Positions for a Subsequent Pass

Setting Load and Store Actions

## Discussion

If your app doesn’t need the data in the texture after completing the rendering pass, use the MTLStoreAction.dontCare action. Otherwise, use the MTLStoreAction.store action if the texture is directly stored or the MTLStoreAction.multisampleResolve action if the texture is a multisampled texture. In some feature sets, you can use the MTLStoreAction.storeAndMultisampleResolve action to store and resolve the texture in a single rendering pass. For more information, see:

- Metal feature set tables (PDF)

- Metal feature set tables (Numbers)

When the store action is either MTLStoreAction.multisampleResolve or MTLStoreAction.storeAndMultisampleResolve, the resolveTexture property must be set to the texture to use as the target for the resolve action. Use the resolveLevel, resolveSlice, and resolveDepthPlane properties to specify the mipmap level, cube slice, and depth plane of the resolve texture, respectively.

For color render targets, the default value is MTLStoreAction.store. For depth or stencil render targets, the default value is MTLStoreAction.dontCare.

## See Also

### Specifying Rendering Pass Actions

var loadAction: MTLLoadAction

The action performed by this attachment at the start of a rendering pass for a render command encoder.

var storeActionOptions: MTLStoreActionOptions

The options that modify the store action performed by this attachment.

