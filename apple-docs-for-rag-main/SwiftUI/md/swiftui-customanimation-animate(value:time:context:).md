

- SwiftUI
- CustomAnimation
-  animate(value:time:context:) 

Instance Method

# animate(value:time:context:)

Calculates the value of the animation at the specified time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func animate(
    value: V,
    time: TimeInterval,
    context: inout AnimationContext
) -> V? where V : VectorArithmetic
```

**Required**

## Parameters 

`value`  

The vector to animate towards.

`time`  

The elapsed time since the start of the animation.

`context`  

An instance of AnimationContext that provides access to state and the animation environment.

## Return Value

The current value of the animation, or `nil` if the animation has finished.

## Discussion

Implement this method to calculate and return the value of the animation at a given point in time. If the animation has finished, return `nil` as the value. This signals to the system that it can remove the animation.

If your custom animation needs to maintain state between calls to the `animate(value:time:context:)` method, store the state data in `context`. This makes the data available to the method next time the system calls it. To learn more about managing state data in a custom animation, see AnimationContext.

