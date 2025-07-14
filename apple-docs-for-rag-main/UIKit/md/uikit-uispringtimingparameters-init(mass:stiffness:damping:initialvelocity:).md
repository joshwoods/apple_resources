

- UIKit
- UISpringTimingParameters
-  init(mass:stiffness:damping:initialVelocity:) 

Initializer

# init(mass:stiffness:damping:initialVelocity:)

Creates a timing parameters object with the specified spring stiffness, mass, damping coefficient, and initial velocity.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init(
    mass: CGFloat,
    stiffness: CGFloat,
    damping: CGFloat,
    initialVelocity velocity: CGVector
)
```

## Parameters 

`mass`  

The effective mass of the animated property. This value must be greater than `0`.

`stiffness`  

The spring stiffness coefficient. Higher values correspond to a stiffer spring that yields a greater amount of force for moving objects.

`damping`  

The damping force to apply to the spring’s motion. This value is used to compute the damping ratio.

`velocity`  

The target property’s initial rate of change at the start of the spring animation. If the target property doesn’t change, specify a vector with `dx` and `dy` components of `0`.

For details about how to calculate this velocity, see initialVelocity.

## Return Value

An initialized spring timing parameters object or `nil` if the object could not be created.

## Discussion

The damping ratio for the spring is computed from the formula `damping` / (2 \* sqrt (`stiffness` \* `mass`)).

## See Also

### Initializing a spring timing parameters object

init()

Creates a default timing parameters object.

convenience init(dampingRatio: CGFloat)

Creates a timing parameters object with the specified damping ratio.

init(dampingRatio: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified damping ratio and initial velocity.

init?(coder: NSCoder)

Creates a timing parameters object from data in an unarchiver.

