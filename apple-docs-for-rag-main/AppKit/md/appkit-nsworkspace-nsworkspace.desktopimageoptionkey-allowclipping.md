

- AppKit
- NSWorkspace
- NSWorkspace.DesktopImageOptionKey
-  allowClipping 

Type Property

# allowClipping

A key that contains the behavior to use when clipping the image.

macOS 10.6+

``` source
static let allowClipping: NSWorkspace.DesktopImageOptionKey
```

## Discussion

The value is an NSNumber containing a Boolean, which affects the interpretation of Proportional scaling types. When the value is false, the workspace object makes the image fully visible, but it may include empty space on the sides or top and bottom. When the value is true, the image fills the entire screen, but may be clipped. If you don’t specify this key, the workspace assumes a value of false. Non-proportional scaling types ignore this value.

## See Also

### Option Keys

static let imageScaling: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when scaling the image.

static let fillColor: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when filling the empty space around the image.

