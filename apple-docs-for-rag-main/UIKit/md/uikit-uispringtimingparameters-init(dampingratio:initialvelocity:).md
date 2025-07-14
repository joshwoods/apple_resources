

- UIKit
- UISpringTimingParameters
-  init(dampingRatio:initialVelocity:) 

Initializer

# init(dampingRatio:initialVelocity:)

Creates a timing parameters object with the specified damping ratio and initial velocity.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init(
    dampingRatio ratio: CGFloat,
    initialVelocity velocity: CGVector
)
```

## Parameters 

`ratio`  

The damping ratio to apply to the spring’s motion. To smoothly decelerate the animation without oscillation, specify a value of `1`. Specify values closer to `0` to create less damping and more oscillation.

`velocity`  

The target property’s initial rate of change at the start of the spring animation. If the target property doesn’t change, specify a vector with `dx` and `dy` components of `0`.

For details about how to calculate this velocity, see initialVelocity.

## Return Value

An initialized spring timing parameters object or `nil` if the object could not be created.

## See Also

### Initializing a spring timing parameters object

init()

Creates a default timing parameters object.

convenience init(dampingRatio: CGFloat)

Creates a timing parameters object with the specified damping ratio.

init(mass: CGFloat, stiffness: CGFloat, damping: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified spring stiffness, mass, damping coefficient, and initial velocity.

init?(coder: NSCoder)

Creates a timing parameters object from data in an unarchiver.

