

- SwiftUI
- AnimationState
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the state for a custom key.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
subscript(key: K.Type) -> K.Value where K : AnimationStateKey { get set }
```

## Overview

Create a custom animation state value by defining a key that conforms to the AnimationStateKey protocol and provide the defaultValue for the key. Also include properties to read and write state values that your CustomAnimation uses. For example, the following code defines a key named `PausableState` that has two state values, `paused` and `pauseTime`:

```
private struct PausableState: AnimationStateKey {
    var paused = false
    var pauseTime: TimeInterval = 0.0

    static var defaultValue: Self { .init() }
}
```

Use that key with the subscript operator of the AnimationState structure to get and set a value for the key. For more convenient access to the key value, extend AnimationContext with a computed property that gets and sets the key’s value.

```
extension AnimationContext {
    fileprivate var pausableState: PausableState {
        get { state[PausableState.self] }
        set { state[PausableState.self] = newValue }
    }
}
```

To access the state values in a CustomAnimation, call the custom computed property, then read and write the state values that the custom AnimationStateKey provides.

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

