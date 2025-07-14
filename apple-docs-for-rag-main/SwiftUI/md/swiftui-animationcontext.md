

- SwiftUI
-  AnimationContext 

Structure

# AnimationContext

Contextual values that a custom animation can use to manage state and access a view’s environment.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AnimationContext where Value : VectorArithmetic
```

## Overview

The system provides an `AnimationContext` to a CustomAnimation instance so that the animation can store and retrieve values in an instance of AnimationState. To access these values, use the context’s state property.

For more convenient access to state, create an AnimationStateKey and extend `AnimationContext` to include a computed property that gets and sets the AnimationState value. Then use this property instead of state to retrieve the state of a custom animation. For example, the following code creates an animation state key named `PausableState`. Then the code extends `AnimationContext` to include the `pausableState` property:

```
private struct PausableState: AnimationStateKey {
    var paused = false
    var pauseTime: TimeInterval = 0.0

    static var defaultValue: Self { .init() }
}

extension AnimationContext {
    fileprivate var pausableState: PausableState {
        get { state[PausableState.self] }
        set { state[PausableState.self] = newValue }
    }
}
```

To access the pausable state, the custom animation `PausableAnimation` uses the `pausableState` property instead of the state property:

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

The animation can also retrieve environment values of the view that created the animation. To retrieve a view’s environment value, use the context’s environment property. For instance, the following code creates a custom EnvironmentValues property named `animationPaused`, and the view `PausableAnimationView` uses the property to store the paused state:

```
extension EnvironmentValues {
    @Entry var animationPaused: Bool = false
}

struct PausableAnimationView: View {
    @State private var paused = false

    var body: some View {
        VStack {
            ...
        }
        .environment(\.animationPaused, paused)
    }
}
```

Then the custom animation `PausableAnimation` retrieves the paused state from the view’s environment using the environment property:

```
struct PausableAnimation: CustomAnimation {
    func animate(value: V, time: TimeInterval, context: inout AnimationContext) -> V? where V : VectorArithmetic {
        let paused = context.environment.animationPaused
        ...
    }
}
```

## Topics

### Managing state

var state: AnimationState&lt;Value>

The current state of a custom animation.

### Retrieving view environment values

var environment: EnvironmentValues

The current environment of the view that created the custom animation.

### Creating context

func withState&lt;T>(AnimationState&lt;T>) -> AnimationContext&lt;T>

Creates a new context from another one with a state that you provide.

### Instance Properties

var isLogicallyComplete: Bool

Set this to `true` to indicate that an animation is logically complete.

## See Also

### Creating custom animations

protocol CustomAnimation

A type that defines how an animatable value changes over time.

struct AnimationState

A container that stores the state for a custom animation.

protocol AnimationStateKey

A key for accessing animation state values.

struct UnitCurve

A function defined by a two-dimensional curve that maps an input progress in the range \[0,1\] to an output progress that is also in the range \[0,1\]. By changing the shape of the curve, the effective speed of an animation or other interpolation can be changed.

struct Spring

A representation of a spring’s motion.

