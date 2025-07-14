

- GameplayKit
- GKState
-  stateMachine 

Instance Property

# stateMachine

The state machine that owns this state object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
weak var stateMachine: GKStateMachine? { get }
```

## Discussion

Use this property to refer to the state machine this state object is being used in.

## See Also

### Working with State Machines

func isValidNextState(AnyClass) -> Bool

Returns a Boolean value indicating whether a state machine currently in this state is allowed to transition into the specified state.

