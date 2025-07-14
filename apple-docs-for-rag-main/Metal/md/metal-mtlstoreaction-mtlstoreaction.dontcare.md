

- Metal
- MTLStoreAction
-  MTLStoreAction.dontCare 

Case

# MTLStoreAction.dontCare

The GPU has permission to discard the rendered contents of the attachment at the end of the render pass, replacing them with arbitrary data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
case dontCare
```

## Mentioned in 

Setting Load and Store Actions

## Discussion

Use this option when you need the attachment’s contents during the render pass but not afterwards. Some GPUs may still store the contents back to the texture, but you can’t rely on that behavior. You must assume that GPU discarded the texture’s contents.

## See Also

### Constants

case store

The GPU stores the rendered contents to the texture.

case multisampleResolve

The GPU resolves the multisampled data to one sample per pixel and stores the data to the resolve texture, discarding the multisample data afterwards.

case storeAndMultisampleResolve

The GPU stores the multisample data to the multisample texture, resolves the data to a sample per pixel, and stores the data to the resolve texture.

case unknown

The system selects a store action when it encodes the render pass.

case customSampleDepthStore

The GPU stores depth data in a sample-position–agnostic representation.

