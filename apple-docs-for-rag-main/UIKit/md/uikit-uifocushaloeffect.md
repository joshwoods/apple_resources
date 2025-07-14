

- UIKit
-  UIFocusHaloEffect 

Class

# UIFocusHaloEffect

A visual focus effect that draws a halo around the focus item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
class UIFocusHaloEffect
```

## Topics

### Creating a halo effect

convenience init(roundedRect: CGRect, cornerRadius: CGFloat, curve: CALayerCornerCurve)

Creates a rounded halo effect using the specified corner radius and corner curve.

convenience init(rect: CGRect)

Creates a rectangular halo effect using the specified rectangle.

convenience init(path: UIBezierPath)

Creates a halo effect using the specified Bézier path.

### Configuring a halo effect

var containerView: UIView?

The container view to place the halo effect into.

var referenceView: UIView?

The view to place the halo effect above.

var position: UIFocusHaloEffect.Position

The position of the halo effect relative to its shape.

enum Position

Constants that describe positions for drawing the halo focus effect.

## Relationships

### Inherits From

- UIFocusEffect

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Focus effects

class UIFocusEffect

The base class for defining a visual focus effect.

enum Position

Constants that describe positions for drawing the halo focus effect.

