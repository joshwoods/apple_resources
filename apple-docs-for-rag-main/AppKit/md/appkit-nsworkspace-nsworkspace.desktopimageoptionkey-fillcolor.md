

- AppKit
- NSWorkspace
- NSWorkspace.DesktopImageOptionKey
-  fillColor 

Type Property

# fillColor

A key that contains the behavior to use when filling the empty space around the image.

macOS 10.6+

``` source
static let fillColor: NSWorkspace.DesktopImageOptionKey
```

## Discussion

The value is the NSColor object to use when filling any empty space around the image. If you don’t specify this key, the workspace object uses a default color. Currently, the system supports only colors that use or can be converted to use the calibratedRGB color space. The system also ignores any alpha value in the color you specify.

## See Also

### Option Keys

static let imageScaling: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when scaling the image.

static let allowClipping: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when clipping the image.

