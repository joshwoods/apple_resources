

- GameplayKit
- GKStateMachine
-  currentState 

Instance Property

# currentState

The state machine’s current state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var currentState: GKState? { get }
```

## Discussion

A state machine can be in only one of its states at a time. To transition to another state, call the enter(_:) method.

When you call the update(deltaTime:) method, the state machine calls the update(deltaTime:) method on its current state object.

## See Also

### Working with States

func canEnterState(AnyClass) -> Bool

Returns a Boolean value indicating whether it is valid for the state machine to transition from its current state to a state of the specified class.

func enter(AnyClass) -> Bool

Attempts to transition the state machine from its current state to a state of the specified class.

func update(deltaTime: TimeInterval)

Tells the current state object to perform per-frame updates.

