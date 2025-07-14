

- UIKit
- UIScreen
- UIScreen.OverscanCompensation
-  insetApplicationFrame Deprecated

Type Property

# insetApplicationFrame

The application frame is reduced in size to compensate for overscan. Content drawn outside the application frame may be clipped.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
static var insetApplicationFrame: UIScreen.OverscanCompensation { get }
```

## See Also

### Constants

case scale

The final composited framebuffer for the screen is scaled so that all pixels lie in the area visible on the screen.

case insetBounds

The screen bounds are reduced in size so that all pixels in the framebuffer are visible on the screen.

case none

No scaling occurs. Use overscanCompensationInsets to get the insets required to avoid clipping.

