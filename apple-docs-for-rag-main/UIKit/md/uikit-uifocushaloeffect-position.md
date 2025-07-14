

- UIKit
- UIFocusHaloEffect
-  position 

Instance Property

# position

The position of the halo effect relative to its shape.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var position: UIFocusHaloEffect.Position { get set }
```

## Discussion

The default value of this property is UIFocusHaloEffect.Position.automatic.

## See Also

### Configuring a halo effect

var containerView: UIView?

The container view to place the halo effect into.

var referenceView: UIView?

The view to place the halo effect above.

enum Position

Constants that describe positions for drawing the halo focus effect.

