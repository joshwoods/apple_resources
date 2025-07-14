

- Metal
- MTLStoreAction
-  MTLStoreAction.storeAndMultisampleResolve 

Case

# MTLStoreAction.storeAndMultisampleResolve

The GPU stores the multisample data to the multisample texture, resolves the data to a sample per pixel, and stores the data to the resolve texture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
case storeAndMultisampleResolve
```

## Mentioned in 

Setting Load and Store Actions

## See Also

### Constants

case dontCare

The GPU has permission to discard the rendered contents of the attachment at the end of the render pass, replacing them with arbitrary data.

case store

The GPU stores the rendered contents to the texture.

case multisampleResolve

The GPU resolves the multisampled data to one sample per pixel and stores the data to the resolve texture, discarding the multisample data afterwards.

case unknown

The system selects a store action when it encodes the render pass.

case customSampleDepthStore

The GPU stores depth data in a sample-position–agnostic representation.

