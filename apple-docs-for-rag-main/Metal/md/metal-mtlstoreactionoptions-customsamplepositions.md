

- Metal
- MTLStoreActionOptions
-  customSamplePositions 

Type Property

# customSamplePositions

An option that stores data in a sample-position–agnostic representation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static var customSamplePositions: MTLStoreActionOptions { get }
```

## Mentioned in 

Storing Data a Pass Makes with Custom Sample Positions for a Subsequent Pass

## Discussion

Set this option only on a MTLRenderPassColorAttachmentDescriptor or MTLRenderPassDepthAttachmentDescriptor object. Setting this option on a MTLRenderPassStencilAttachmentDescriptor object or combining it with a nonstore storeAction value results in a runtime error.

Set this action when you need to read the data in a subsequent render pass or blit operation that is unaware of the programmable sample positions used to generate the data. You should set this option when, for example, reading per-sample data within a fragment function that uses different programmable sample positions.

If you specify this action, Metal may decompress the depth render target and store the resulting data in its decompressed form. If you don’t change programmable sample positions in a subsequent render pass, use MTLStoreAction.store instead to improve performance.

## See Also

### Constants

init(rawValue: UInt)

Creates a store action option from a raw integer value.

