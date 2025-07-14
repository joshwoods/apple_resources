

- UIKit
- UIFocusHaloEffect
-  referenceView 

Instance Property

# referenceView

The view to place the halo effect above.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
weak var referenceView: UIView? { get set }
```

## Discussion

If you set this property, the halo effect appears above this view. If you also set containerView, this reference view must be a descendant of the container view. The system ensures that the halo effect is in the container but visually above the reference view.

## See Also

### Configuring a halo effect

var containerView: UIView?

The container view to place the halo effect into.

var position: UIFocusHaloEffect.Position

The position of the halo effect relative to its shape.

enum Position

Constants that describe positions for drawing the halo focus effect.

