

- AppKit
- NSImageView
-  defaultPreferredImageDynamicRange 

Type Property

# defaultPreferredImageDynamicRange

The default preferred image dynamic range.

macOS 14.0+

``` source
@MainActor
class var defaultPreferredImageDynamicRange: NSImage.DynamicRange { get set }
```

## Discussion

This property defaults to NSImage.DynamicRange.constrainedHigh on macOS 14 and higher, and NSImage.DynamicRange.standard otherwise. Set this property to another NSImage.DynamicRange value to change the default for all subsequently created image views in your app.

## See Also

### Specifying the dynamic range

var imageDynamicRange: NSImage.DynamicRange

The resolved dynamic range of the fully resolved image content.

var preferredImageDynamicRange: NSImage.DynamicRange

The preferred dynamic range when displaying an image in the receiving image view.

