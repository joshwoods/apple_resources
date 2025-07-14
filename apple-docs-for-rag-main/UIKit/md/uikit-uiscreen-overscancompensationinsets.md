

- UIKit
- UIScreen
-  overscanCompensationInsets 

Instance Property

# overscanCompensationInsets

The edge inset values needed to avoid clipping the rectangle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+

``` source
@MainActor
var overscanCompensationInsets: UIEdgeInsets { get }
```

## See Also

### Managing overscan compensation

var overscanCompensation: UIScreen.OverscanCompensation

For an external screen, this property sets the desired technique to compensate for overscan.

enum OverscanCompensation

Describes different techniques for compensating for pixel loss at the edge of the screen.

