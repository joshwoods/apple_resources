

- UIKit
- UIFieldBehavior
-  strength 

Instance Property

# strength

The strength of the field.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var strength: CGFloat { get set }
```

## Discussion

The default value of this property is `1.0`. The effect of this value is dependent on the type of field. In practice, the best approach for determining the strength of the field you want is to experiment with different values until you get the behavior you want.

## See Also

### Configuring the field attributes

var position: CGPoint

The position of the field in the reference coordinate system.

var region: UIRegion

The shape of the field.

var falloff: CGFloat

The rate of decay for the field strength.

var minimumRadius: CGFloat

The minimum distance at which to start calculating new values for the field.

var direction: CGVector

The direction of motion for a linear field.

var smoothness: CGFloat

The smoothness of the noise used to generate the field.

var animationSpeed: CGFloat

The rate at which the animation should proceed.

