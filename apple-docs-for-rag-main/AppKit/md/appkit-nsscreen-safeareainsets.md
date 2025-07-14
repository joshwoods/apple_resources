

- AppKit
- NSScreen
-  safeAreaInsets 

Instance Property

# safeAreaInsets

The distances from the screen’s edges at which content isn’t obscured.

macOS 12.0+

``` source
var safeAreaInsets: NSEdgeInsets { get }
```

## Discussion

The safe area reflects the unobscured portion of the screen. On some Macs, the insets reflect the portion of the screen covered by the camera housing. If your app offers a custom full-screen experience, apply the specified insets to the screen’s frame rectangle to obtain the area within which it is safe to display your content. Content in the safe area is guaranteed to be unobscured.

If your app uses the system’s full-screen experience, you don’t need to account for the safe area in your window. When you call your window’s toggleFullScreen(_:) method to enter full-screen mode, the system automatically positions the window’s contents within the safe area.

## See Also

### Getting the Visible Portion of the Screen

var visibleFrame: NSRect

The current location and dimensions of the visible screen.

var auxiliaryTopLeftArea: NSRect?

The unobscured portion of the top-left corner of the screen.

var auxiliaryTopRightArea: NSRect?

The unobscured portion of the top-right corner of the screen.

