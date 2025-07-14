

- AppKit
- NSMagnificationGestureRecognizer
-  magnification 

Instance Property

# magnification

The amount of magnification to apply.

macOS 10.10+

``` source
@MainActor
var magnification: CGFloat { get set }
```

## Discussion

This property contains the current magnification in effect for the gesture. Add the value of this property to `1.0` to get the scale factor to apply to your content.

