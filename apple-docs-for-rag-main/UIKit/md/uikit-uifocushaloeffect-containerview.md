

- UIKit
- UIFocusHaloEffect
-  containerView 

Instance Property

# containerView

The container view to place the halo effect into.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
weak var containerView: UIView? { get set }
```

## Discussion

If you don’t set this property, the system automatically determines the container according to the focus item that provides the effect and referenceView, if present.

## See Also

### Configuring a halo effect

var referenceView: UIView?

The view to place the halo effect above.

var position: UIFocusHaloEffect.Position

The position of the halo effect relative to its shape.

enum Position

Constants that describe positions for drawing the halo focus effect.

