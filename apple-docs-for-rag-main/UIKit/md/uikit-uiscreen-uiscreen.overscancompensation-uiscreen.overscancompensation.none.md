

- UIKit
- UIScreen
- UIScreen.OverscanCompensation
-  UIScreen.OverscanCompensation.none 

Case

# UIScreen.OverscanCompensation.none

No scaling occurs. Use overscanCompensationInsets to get the insets required to avoid clipping.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+

``` source
case none
```

## See Also

### Constants

case scale

The final composited framebuffer for the screen is scaled so that all pixels lie in the area visible on the screen.

case insetBounds

The screen bounds are reduced in size so that all pixels in the framebuffer are visible on the screen.

static var insetApplicationFrame: UIScreen.OverscanCompensation

The application frame is reduced in size to compensate for overscan. Content drawn outside the application frame may be clipped.

Deprecated

