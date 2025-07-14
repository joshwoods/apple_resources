

- AppKit
- NSWorkspace
- NSWorkspace.DesktopImageOptionKey
-  imageScaling 

Type Property

# imageScaling

A key that contains the behavior to use when scaling the image.

macOS 10.6+

``` source
static let imageScaling: NSWorkspace.DesktopImageOptionKey
```

## Discussion

The value is an NSNumber object that contains an NSImageScaling constant as declared in NSCell. If you don’t include this key, the workspace object uses NSImageScaling.scaleProportionallyUpOrDown. NSImageScaling.scaleProportionallyDown isn’t supported.

## See Also

### Option Keys

static let allowClipping: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when clipping the image.

static let fillColor: NSWorkspace.DesktopImageOptionKey

A key that contains the behavior to use when filling the empty space around the image.

