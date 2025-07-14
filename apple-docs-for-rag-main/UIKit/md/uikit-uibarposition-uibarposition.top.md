

- UIKit
- UIBarPosition
-  UIBarPosition.top 

Case

# UIBarPosition.top

Specifies that the bar is at the top of its containing view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case top
```

## Discussion

The system uses this as a hint to draw directional decoration accordingly. For example, any shadow would be drawn below the bar.

Instances of UIToolbar do not appear with this position on iPhone, but they can on iPad.

## See Also

### Constants

case any

Specifies that the position is unspecified.

case bottom

Specifies that the bar is at the bottom of its containing view.

case topAttached

Specifies that the bar is at the top of the screen, as well as its containing view.

