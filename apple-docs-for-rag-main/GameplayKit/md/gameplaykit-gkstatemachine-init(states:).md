

- GameplayKit
- GKStateMachine
-  init(states:) 

Initializer

# init(states:)

Initializes a state machine with the specified states.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(states: [GKState])
```

## Parameters 

`states`  

An array of state objects. Each object in the array must be of a unique subclass of GKState.

## Return Value

A new state machine.

## Discussion

The newly created state machine’s currentState property is `nil`. To choose and enter an initial state, use the enter(_:) method.

For more information, see GameplayKit Programming Guide.

