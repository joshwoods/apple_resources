

- SwiftUI
- AnimationContext
-  state 

Instance Property

# state

The current state of a custom animation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var state: AnimationState
```

## Discussion

An instance of CustomAnimation uses this property to read and write state values as the animation runs.

An alternative to using the `state` property in a custom animation is to create an AnimationStateKey type and extend AnimationContext with a custom property that returns the state as a custom type. For example, the following code creates a state key named `PausableState`. It’s convenient to store state values in the key type, so the `PausableState` structure includes properties for the stored state values `paused` and `pauseTime`.

```
private struct PausableState: AnimationStateKey {
    var paused = false
    var pauseTime: TimeInterval = 0.0

    static var defaultValue: Self { .init() }
}
```

To provide access the pausable state, the following code extends `AnimationContext` to include the `pausableState` property. This property returns an instance of the custom `PausableState` structure stored in state, and it can also store a new `PausableState` instance in `state`.

```
extension AnimationContext {
    fileprivate var pausableState: PausableState {
        get { state[PausableState.self] }
        set { state[PausableState.self] = newValue }
    }
}
```

Now a custom animation can use the `pausableState` property instead of the state property as a convenient way to read and write state values as the animation runs.

```
struct PausableAnimation: CustomAnimation {
    func animate(value: V, time: TimeInterval, context: inout AnimationContext) -> V? where V : VectorArithmetic {
        let pausableState = context.pausableState
        var pauseTime = pausableState.pauseTime
        ...
    }
}
```

