

- Metal
- MTLRenderPassAttachmentDescriptor
-  loadAction 

Instance Property

# loadAction

The action performed by this attachment at the start of a rendering pass for a render command encoder.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var loadAction: MTLLoadAction { get set }
```

## Mentioned in 

Setting Load and Store Actions

## Discussion

If your app renders all pixels of the render target for a given frame, use the MTLLoadAction.dontCare action, which allows the GPU to avoid loading the existing contents of the texture. Otherwise, use the MTLLoadAction.clear action to clear the previous contents of the render target or the MTLLoadAction.load action to preserve them. The MTLLoadAction.clear action also avoids the cost of loading the existing texture contents, but it still incurs the cost of filling the destination with a clear color.

For color render targets, the default value is MTLLoadAction.dontCare. For depth or stencil render targets, the default value is MTLLoadAction.clear.

## See Also

### Specifying Rendering Pass Actions

var storeAction: MTLStoreAction

The action performed by this attachment at the end of a rendering pass for a render command encoder.

var storeActionOptions: MTLStoreActionOptions

The options that modify the store action performed by this attachment.

