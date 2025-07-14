

- UIKit
- UIFieldBehavior
-  direction 

Instance Property

# direction

The direction of motion for a linear field.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var direction: CGVector { get set }
```

## Discussion

Use this property to specify the direction of motion for velocity and linear gravity fields. For nondirectional fields, the default value of this property is a zero vector.

## See Also

### Configuring the field attributes

var position: CGPoint

The position of the field in the reference coordinate system.

var region: UIRegion

The shape of the field.

var strength: CGFloat

The strength of the field.

var falloff: CGFloat

The rate of decay for the field strength.

var minimumRadius: CGFloat

The minimum distance at which to start calculating new values for the field.

var smoothness: CGFloat

The smoothness of the noise used to generate the field.

var animationSpeed: CGFloat

The rate at which the animation should proceed.

