

- UIKit
- UIFieldBehavior
-  vortexField() 

Type Method

# vortexField()

Creates and returns a field behavior object that applies a rotational force relative to the field’s position.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class func vortexField() -> Self
```

## Return Value

A field behavior object that applies a rotational force around the field’s origin.

## Discussion

This forces created by this field rotate in a circle around the center point of the field. Items entering the field are pushed perpendicular to the imaginary line between the item and the center of the field. Combine this field with a radial gravity field to create a field that pulls items into a spinning vortex.

When setting the strength of the vortex field, positive values create a counter-clockwise rotation and negative values create a clockwise rotation. The amount of force is proportional to the item’s mass and the item’s distance from the field’s origin.

## See Also

### Getting the field behaviors

class func dragField() -> Self

Creates and returns a field behavior for slowing an object’s velocity.

class func springField() -> Self

Creates and returns a spring field behavior.

class func velocityField(direction: CGVector) -> Self

Creates and returns a field behavior object that applies a directional velocity to items.

class func electricField() -> Self

Creates and returns a field behavior object that interacts with charged items.

class func magneticField() -> Self

Creates and returns a field behavior that interacts with charged items.

class func radialGravityField(position: CGPoint) -> Self

Creates and returns a field behavior object that models a radial gravitational force.

class func linearGravityField(direction: CGVector) -> Self

Creates and returns a field behavior object that models a linear gravitational force.

class func noiseField(smoothness: CGFloat, animationSpeed: CGFloat) -> Self

Creates and returns a field behavior object that applies random noise to other forces.

class func turbulenceField(smoothness: CGFloat, animationSpeed: CGFloat) -> Self

Creates and returns a field behavior object that applies noise to an item in motion.

class func field(evaluationBlock: (UIFieldBehavior, CGPoint, CGVector, CGFloat, CGFloat, TimeInterval) -> CGVector) -> Self

Creates and returns a field behavior object that applies an app-specified field to items.

