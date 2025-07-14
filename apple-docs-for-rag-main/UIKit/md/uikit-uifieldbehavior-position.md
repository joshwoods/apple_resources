

- UIKit
- UIFieldBehavior
-  position 

Instance Property

# position

The position of the field in the reference coordinate system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var position: CGPoint { get set }
```

## Discussion

This property defines the center point of the field. The shape of the field around this point is defined by the region property.

## See Also

### Configuring the field attributes

var region: UIRegion

The shape of the field.

var strength: CGFloat

The strength of the field.

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

