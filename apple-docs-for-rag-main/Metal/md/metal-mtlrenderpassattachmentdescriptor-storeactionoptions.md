

- Metal
- MTLRenderPassAttachmentDescriptor
-  storeActionOptions 

Instance Property

# storeActionOptions

The options that modify the store action performed by this attachment.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var storeActionOptions: MTLStoreActionOptions { get set }
```

## Mentioned in 

Storing Data a Pass Makes with Custom Sample Positions for a Subsequent Pass

## Discussion

This property specifies additional behavior for the store action specified by the storeAction property.

The default value is MTLStoreActionOptionNone.

## See Also

### Specifying Rendering Pass Actions

var loadAction: MTLLoadAction

The action performed by this attachment at the start of a rendering pass for a render command encoder.

var storeAction: MTLStoreAction

The action performed by this attachment at the end of a rendering pass for a render command encoder.

