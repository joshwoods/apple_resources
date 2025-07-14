

- UIKit
- UISpringTimingParameters
-  init(coder:) 

Initializer

# init(coder:)

Creates a timing parameters object from data in an unarchiver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Initializing a spring timing parameters object

init()

Creates a default timing parameters object.

convenience init(dampingRatio: CGFloat)

Creates a timing parameters object with the specified damping ratio.

init(dampingRatio: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified damping ratio and initial velocity.

init(mass: CGFloat, stiffness: CGFloat, damping: CGFloat, initialVelocity: CGVector)

Creates a timing parameters object with the specified spring stiffness, mass, damping coefficient, and initial velocity.

