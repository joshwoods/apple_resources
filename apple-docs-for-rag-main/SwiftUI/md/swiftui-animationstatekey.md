

- SwiftUI
-  AnimationStateKey 

Protocol

# AnimationStateKey

A key for accessing animation state values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol AnimationStateKey
```

## Overview

To access animation state from an AnimationContext in a custom animation, create an `AnimationStateKey`. For example, the following code creates an animation state key named `PausableState` and sets the value for the required defaultValue property. The code also defines properties for state values that the custom animation needs when calculating animation values. Keeping the state values in the animation state key makes it more convenient to read and write those values in the implementation of a CustomAnimation.

```
private struct PausableState: AnimationStateKey {
    var paused = false
    var pauseTime: TimeInterval = 0.0

    static var defaultValue: Self { .init() }
}
```

To make accessing the value of the animation state key more convenient, define a property for it by extending AnimationContext:

```
extension AnimationContext {
    fileprivate var pausableState: PausableState {
        get { state[PausableState.self] }
        set { state[PausableState.self] = newValue }
    }
}
```

Then, you can read and write your state in an instance of `CustomAnimation` using the AnimationContext:

```
struct PausableAnimation: CustomAnimation {
    let base: Animation

    func animate(value: V, time: TimeInterval, context: inout AnimationContext) -> V? where V : VectorArithmetic {
        let paused = context.environment.animationPaused

        let pausableState = context.pausableState
        var pauseTime = pausableState.pauseTime
        if pausableState.paused != paused {
            pauseTime = time - pauseTime
            context.pausableState = PausableState(paused: paused, pauseTime: pauseTime)
        }

        let effectiveTime = paused ? pauseTime : time - pauseTime
        let result = base.animate(value: value, time: effectiveTime, context: &context)
        return result
    }
}
```

## Topics

### Setting the default value

static var defaultValue: Self.Value

The default value for the animation state key.

**Required**

associatedtype Value

The associated type representing the type of the animation state key’s value.

**Required**

## See Also

### Creating custom animations

protocol CustomAnimation

A type that defines how an animatable value changes over time.

struct AnimationContext

Contextual values that a custom animation can use to manage state and access a view’s environment.

struct AnimationState

A container that stores the state for a custom animation.

struct UnitCurve

A function defined by a two-dimensional curve that maps an input progress in the range \[0,1\] to an output progress that is also in the range \[0,1\]. By changing the shape of the curve, the effective speed of an animation or other interpolation can be changed.

struct Spring

A representation of a spring’s motion.

