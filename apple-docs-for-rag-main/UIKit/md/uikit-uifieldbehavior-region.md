

- UIKit
- UIFieldBehavior
-  region 

Instance Property

# region

The shape of the field.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var region: UIRegion { get set }
```

## Discussion

This property defines the shape of the field centered on the point in the position property. A field does not exert any force on items that lie outside of the specified region.

## See Also

### Configuring the field attributes

var position: CGPoint

The position of the field in the reference coordinate system.

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

