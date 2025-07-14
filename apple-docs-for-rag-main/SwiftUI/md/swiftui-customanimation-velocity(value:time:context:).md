

- SwiftUI
- CustomAnimation
-  velocity(value:time:context:) 

Instance Method

# velocity(value:time:context:)

Calculates the velocity of the animation at a specified time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func velocity(
    value: V,
    time: TimeInterval,
    context: AnimationContext
) -> V? where V : VectorArithmetic
```

**Required** Default implementation provided.

## Parameters 

`value`  

The vector to animate towards.

`time`  

The amount of time since the start of the animation.

`context`  

An instance of AnimationContext that provides access to state and the animation environment.

## Return Value

The current velocity of the animation, or `nil` if the animation has finished.

## Discussion

Implement this method to provide the velocity of the animation at a given time. Should subsequent animations merge with the animation, the system preserves continuity of the velocity between animations.

The default implementation of this method returns `nil`.

Note

State and environment data is available to this method via the `context` parameter, but `context` is read-only. This behavior is different than with animate(value:time:context:) and shouldMerge(previous:value:time:context:) where `context` is an `inout` parameter, letting you change the context including state data of the animation. For more information about managing state data in a custom animation, see AnimationContext.

## Default Implementations

### CustomAnimation Implementations

func velocity&lt;V>(value: V, time: TimeInterval, context: AnimationContext&lt;V>) -> V?

Calculates the velocity of the animation at a specified time.

