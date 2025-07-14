

- GameplayKit
- GKStateMachine
-  canEnterState(\_:) 

Instance Method

# canEnterState(\_:)

Returns a Boolean value indicating whether it is valid for the state machine to transition from its current state to a state of the specified class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func canEnterState(_ stateClass: AnyClass) -> Bool
```

## Parameters 

`stateClass`  

The class of state for which to determine whether a transition is allowed.

## Return Value

true if a transition is allowed from the current state to a state of the specified class; otherwise false.

## Discussion

You build a state machine by creating a unique GKState subclass for each distinct state possible for the machine. The isValidNextState(_:) method of each state object determines which other states a state machine is allowed to transition into from that state.

A newly created state machine’s currentState property is `nil`. In this case, the canEnterState(_:) method always returns true. To choose and enter an initial state, use the enter(_:) method.

## See Also

### Working with States

var currentState: GKState?

The state machine’s current state.

func enter(AnyClass) -> Bool

Attempts to transition the state machine from its current state to a state of the specified class.

func update(deltaTime: TimeInterval)

Tells the current state object to perform per-frame updates.

