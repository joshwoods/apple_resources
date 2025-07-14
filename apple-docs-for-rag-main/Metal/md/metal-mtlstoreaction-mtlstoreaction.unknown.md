

- Metal
- MTLStoreAction
-  MTLStoreAction.unknown 

Case

# MTLStoreAction.unknown

The system selects a store action when it encodes the render pass.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
case unknown
```

## Mentioned in 

Setting Load and Store Actions

## Discussion

Only apply this action if you can’t determine the store action when you create the render pass descriptor. You must specify a store action before you finish encoding commands into the render command encoder. Refer to the MTLRenderCommandEncoder and MTLParallelRenderCommandEncoder protocol references for further information.

## See Also

### Constants

case dontCare

The GPU has permission to discard the rendered contents of the attachment at the end of the render pass, replacing them with arbitrary data.

case store

The GPU stores the rendered contents to the texture.

case multisampleResolve

The GPU resolves the multisampled data to one sample per pixel and stores the data to the resolve texture, discarding the multisample data afterwards.

case storeAndMultisampleResolve

The GPU stores the multisample data to the multisample texture, resolves the data to a sample per pixel, and stores the data to the resolve texture.

case customSampleDepthStore

The GPU stores depth data in a sample-position–agnostic representation.

