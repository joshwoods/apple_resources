

- UIKit
- UIScreen
-  overscanCompensation 

Instance Property

# overscanCompensation

For an external screen, this property sets the desired technique to compensate for overscan.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var overscanCompensation: UIScreen.OverscanCompensation { get set }
```

## Discussion

Some external displays may be unable to reliably display all of the pixels to the user. To compensate, choose one of the techniques described in the UIScreen.OverscanCompensation enumeration.

## See Also

### Managing overscan compensation

var overscanCompensationInsets: UIEdgeInsets

The edge inset values needed to avoid clipping the rectangle.

enum OverscanCompensation

Describes different techniques for compensating for pixel loss at the edge of the screen.

