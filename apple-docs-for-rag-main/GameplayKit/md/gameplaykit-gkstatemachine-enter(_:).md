

- GameplayKit
- GKStateMachine
-  enter(\_:) 

Instance Method

# enter(\_:)

Attempts to transition the state machine from its current state to a state of the specified class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func enter(_ stateClass: AnyClass) -> Bool
```

## Parameters 

`stateClass`  

The class of state into which to attempt a transition.

## Return Value

true if the transition was successful; otherwise false.

## Discussion

You build a state machine by creating a unique GKState subclass for each distinct state possible for the machine. The isValidNextState(_:) method of each state object determines which other states a state machine is allowed to transition into from that state. Calling this method first tests whether a transition from the current state to the specified state is valid; if not, this method returns false.

If a transition is allowed, the state machine sends the willExit(to:) message to its current state object. Then, the new state object replaces the value of the currentState property. Finally, the state machine sends the didEnter(from:) message to the new current state object, and this method returns true.

A newly created state machine’s currentState property is `nil`—to choose and enter an initial state, use the enter(_:) method. In this case, the enter(_:) call always succeeds.

## See Also

### Working with States

var currentState: GKState?

The state machine’s current state.

func canEnterState(AnyClass) -> Bool

Returns a Boolean value indicating whether it is valid for the state machine to transition from its current state to a state of the specified class.

func update(deltaTime: TimeInterval)

Tells the current state object to perform per-frame updates.

