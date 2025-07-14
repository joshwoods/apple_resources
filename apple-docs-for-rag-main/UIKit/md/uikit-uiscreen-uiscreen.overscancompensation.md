

- UIKit
- UIScreen
-  UIScreen.OverscanCompensation 

Enumeration

# UIScreen.OverscanCompensation

Describes different techniques for compensating for pixel loss at the edge of the screen.

iOSiPadOSMac CatalysttvOS

``` source
enum OverscanCompensation
```

## Topics

### Constants

case scale

The final composited framebuffer for the screen is scaled so that all pixels lie in the area visible on the screen.

case insetBounds

The screen bounds are reduced in size so that all pixels in the framebuffer are visible on the screen.

case none

No scaling occurs. Use overscanCompensationInsets to get the insets required to avoid clipping.

static var insetApplicationFrame: UIScreen.OverscanCompensation

The application frame is reduced in size to compensate for overscan. Content drawn outside the application frame may be clipped.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing overscan compensation

var overscanCompensationInsets: UIEdgeInsets

The edge inset values needed to avoid clipping the rectangle.

var overscanCompensation: UIScreen.OverscanCompensation

For an external screen, this property sets the desired technique to compensate for overscan.

