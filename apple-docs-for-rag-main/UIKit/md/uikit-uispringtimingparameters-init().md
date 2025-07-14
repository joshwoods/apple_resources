

- UIKit
- UISpringTimingParameters
-  init() 

Initializer

# init()

Creates a default timing parameters object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init()
```

## Return Value

An initialized spring timing parameters object or `nil` if the object could not be created.

## Discussion

This method sets the initial velocity of any animated properties to `0.0` and sets the damping ratio to `4.56`.

## See Also

### Initializing a spring timing parameters object

convenience init(dampingRatio: CGFloat)

Creates a timing parameters object with the specified damping ratio.

init(dampingRatio: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified damping ratio and initial velocity.

init(mass: CGFloat, stiffness: CGFloat, damping: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified spring stiffness, mass, damping coefficient, and initial velocity.

init?(coder: NSCoder)

Creates a timing parameters object from data in an unarchiver.

