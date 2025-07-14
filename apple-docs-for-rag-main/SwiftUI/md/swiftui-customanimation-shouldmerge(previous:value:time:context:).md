

- SwiftUI
- CustomAnimation
-  shouldMerge(previous:value:time:context:) 

Instance Method

# shouldMerge(previous:value:time:context:)

Determines whether an instance of the animation can merge with other instance of the same type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func shouldMerge(
    previous: Animation,
    value: V,
    time: TimeInterval,
    context: inout AnimationContext
) -> Bool where V : VectorArithmetic
```

**Required** Default implementation provided.

## Parameters 

`previous`  

The previous running animation.

`value`  

The vector to animate towards.

`time`  

The amount of time since the start of the previous animation.

`context`  

An instance of AnimationContext that provides access to state and the animation environment.

## Return Value

A Boolean value of `true` if the animation should merge with the previous animation; otherwise, `false`.

## Discussion

When a view creates a new animation on an animatable value that already has a running animation of the same animation type, the system calls the `shouldMerge(previous:value:time:context:)` method on the new instance to determine whether it can merge the two instance. Implement this method if the animation can merge with another instance. The default implementation returns `false`.

If `shouldMerge(previous:value:time:context:)` returns `true`, the system merges the new animation instance with the previous animation. The system provides to the new instance the state and elapsed time from the previous one. Then it removes the previous animation.

If this method returns `false`, the system doesn’t merge the animation with the previous one. Instead, both animations run together and the system combines their results.

If your custom animation needs to maintain state between calls to the `shouldMerge(previous:value:time:context:)` method, store the state data in `context`. This makes the data available to the method next time the system calls it. To learn more, see AnimationContext.

## Default Implementations

### CustomAnimation Implementations

func shouldMerge&lt;V>(previous: Animation, value: V, time: TimeInterval, context: inout AnimationContext&lt;V>) -> Bool

Determines whether an instance of the animation can merge with other instance of the same type.

