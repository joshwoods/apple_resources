

- UIKit
- UIFieldBehavior
-  animationSpeed 

Instance Property

# animationSpeed

The rate at which the animation should proceed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var animationSpeed: CGFloat { get set }
```

## Discussion

For noise and turbulence fields, this property contains the speed at which to animate the field. For all other fields, the value of this property is always `0.0`.

A value of `1.0` means the field animations occur at normal speed. Values less than `1.0` result in animations that are slower than normal, and values greater than `1.0` result in animations that are faster than normal. A value of `0.0` means that the field does not animate at all.

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

var smoothness: CGFloat

The smoothness of the noise used to generate the field.

