

- UIKit
- UIFieldBehavior
-  falloff 

Instance Property

# falloff

The rate of decay for the field strength.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var falloff: CGFloat { get set }
```

## Discussion

This property defines how quickly the field strength diminishes as the distance from the field’s center increases. Falloff is not applied until the distance between objects is greater than the value in the minimumRadius property.

The default value of the property is 0, which yields a uniform field that does not diminish over distance.

## See Also

### Configuring the field attributes

var position: CGPoint

The position of the field in the reference coordinate system.

var region: UIRegion

The shape of the field.

var strength: CGFloat

The strength of the field.

var minimumRadius: CGFloat

The minimum distance at which to start calculating new values for the field.

var direction: CGVector

The direction of motion for a linear field.

var smoothness: CGFloat

The smoothness of the noise used to generate the field.

var animationSpeed: CGFloat

The rate at which the animation should proceed.

