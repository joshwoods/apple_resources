

- SwiftUI
- Spring
-  init(settlingDuration:dampingRatio:epsilon:) 

Initializer

# init(settlingDuration:dampingRatio:epsilon:)

Creates a spring with the specified duration and damping ratio.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    settlingDuration: TimeInterval,
    dampingRatio: Double,
    epsilon: Double = 0.001
)
```

## Parameters 

`settlingDuration`  

The approximate time it will take for the spring to come to rest.

`dampingRatio`  

The amount of drag applied as a fraction of the amount needed to produce critical damping.

`epsilon`  

The threshhold for how small all subsequent values need to be before the spring is considered to have settled.

## See Also

### Creating a spring

init(duration: TimeInterval, bounce: Double)

Creates a spring with the specified duration and bounce.

init(mass: Double, stiffness: Double, damping: Double, allowOverDamping: Bool)

Creates a spring with the specified mass, stiffness, and damping.

init(response: Double, dampingRatio: Double)

Creates a spring with the specified response and damping ratio.

