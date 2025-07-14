

- UIKit
- UIFieldBehavior
-  smoothness 

Instance Property

# smoothness

The smoothness of the noise used to generate the field.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var smoothness: CGFloat { get set }
```

## Discussion

For noise and turbulence fields, this value specifies the amount of noise or turbulence. The value of this property is in the range `0.0` to `1.0`, where `0.0` represents the maximum noise or turbulence and `1.0` represents the least amount of noise or turbulence.

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

var direction: CGVector

The direction of motion for a linear field.

var animationSpeed: CGFloat

The rate at which the animation should proceed.

