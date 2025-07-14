

- AppKit
- NSImageView
-  imageDynamicRange 

Instance Property

# imageDynamicRange

The resolved dynamic range of the fully resolved image content.

macOS 14.0+

``` source
@MainActor
var imageDynamicRange: NSImage.DynamicRange { get }
```

## Discussion

This property returns NSImage.DynamicRange.unspecified if the image view can’t resolve the image content or the image view hasn’t displayed.

## See Also

### Specifying the dynamic range

var preferredImageDynamicRange: NSImage.DynamicRange

The preferred dynamic range when displaying an image in the receiving image view.

class var defaultPreferredImageDynamicRange: NSImage.DynamicRange

The default preferred image dynamic range.

