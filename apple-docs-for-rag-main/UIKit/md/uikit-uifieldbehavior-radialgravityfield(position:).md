

- UIKit
- UIFieldBehavior
-  radialGravityField(position:) 

Type Method

# radialGravityField(position:)

Creates and returns a field behavior object that models a radial gravitational force.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class func radialGravityField(position: CGPoint) -> Self
```

## Parameters 

`position`  

The location of the gravitation force in the reference coordinate system. You can change this value later by modifying the position property.

## Return Value

A field behavior object that applies a gravitational force to items with mass.

## Discussion

This field creates a gravitational force at the specified point in the referenced coordinate system. Dynamic items with mass are attracted to the specified point with a force that is proportional to their distance from the point.

When setting the strength of the field, positive values attract items to the field’s position and negative values repel items. The force on the object can be determined by the equation `F = ma`. The force equals the mass of the object multiplied by the acceleration imposed by the gravitational field, which is determined by the strength of the field and the distance of the item from the field’s origin.

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

class func linearGravityField(direction: CGVector) -> Self

Creates and returns a field behavior object that models a linear gravitational force.

class func vortexField() -> Self

Creates and returns a field behavior object that applies a rotational force relative to the field’s position.

class func noiseField(smoothness: CGFloat, animationSpeed: CGFloat) -> Self

Creates and returns a field behavior object that applies random noise to other forces.

class func turbulenceField(smoothness: CGFloat, animationSpeed: CGFloat) -> Self

Creates and returns a field behavior object that applies noise to an item in motion.

class func field(evaluationBlock: (UIFieldBehavior, CGPoint, CGVector, CGFloat, CGFloat, TimeInterval) -> CGVector) -> Self

Creates and returns a field behavior object that applies an app-specified field to items.

