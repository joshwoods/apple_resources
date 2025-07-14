

- UIKit
- UIScreen
- UIScreen.OverscanCompensation
-  UIScreen.OverscanCompensation.scale 

Case

# UIScreen.OverscanCompensation.scale

The final composited framebuffer for the screen is scaled so that all pixels lie in the area visible on the screen.

iOSiPadOSMac CatalysttvOS

``` source
case scale
```

## See Also

### Constants

case insetBounds

The screen bounds are reduced in size so that all pixels in the framebuffer are visible on the screen.

case none

No scaling occurs. Use overscanCompensationInsets to get the insets required to avoid clipping.

static var insetApplicationFrame: UIScreen.OverscanCompensation

The application frame is reduced in size to compensate for overscan. Content drawn outside the application frame may be clipped.

Deprecated

