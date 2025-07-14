

- GameplayKit
-  GKStateMachine 

Class

# GKStateMachine

A finite-state machine—a collection of state objects that each define logic for a particular state of gameplay and rules for transitioning between states.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKStateMachine
```

## Overview

In GameplayKit, you subclass GKState to define each state and the rules for allowed transitions between states, and use a GKStateMachine instance to manage a machine that combines several states. This system provides a way to organize code in your game by organizing state-dependent actions into methods that run when entering a state, when exiting a state, and periodically while in a state (for example, on every animation frame your game renders).

You can use state machines to govern various aspects of a game. For example:

- An enemy character might use a state machine with Chase, Flee, Dead, and Respawn states, each of which drives the enemy’s behavior, with state transitions determined by player actions and elapsed time.

- An automated turret might use a state machine with Ready, Firing, and Cooldown states, controlling when it seeks out nearby targets and how often it fires.

- A game user interface might use Menu, Playing, Paused, and GameOver states, each of which determines what UI elements are shown and what other game elements are running.

To build a state machine, first define a distinct subclass of GKState for each possible state of the machine. In each state class, the isValidNextState(_:) method determines which other state classes the machine may transition into from that state. Then, create a state machine object by constructing instances of the state classes and passing them to one of the methods listed in Creating a State Machine below. Finally, set the machine in motion by choosing an initial state for it to enter with the enter(_:) method.

To define state-dependent behavior, override the didEnter(from:), update(deltaTime:), and willExit(to:) methods in each GKState subclass.

- The state machine notifies the current state whenever a state change happens. Use the didEnter(from:) and willExit(to:) methods to perform actions in response to a state change. For example, an enemy character entering the Flee state might change its appearance to indicate that is has become vulnerable to attack by the player.

- When you call a state machine’s update(deltaTime:) method, the state machine calls the update(deltaTime:) method of its current state. Use this method to organize per-frame update code by state. For example, an enemy character in the Chase state can update its position to pursue the player, and an enemy in the Flee state can update its position to evade the player.

For more information about state machines, read State Machines in GameplayKit Programming Guide.

## Topics

### Creating a State Machine

init(states: [GKState])

Initializes a state machine with the specified states.

### Working with States

var currentState: GKState?

The state machine’s current state.

func canEnterState(AnyClass) -> Bool

Returns a Boolean value indicating whether it is valid for the state machine to transition from its current state to a state of the specified class.

func enter(AnyClass) -> Bool

Attempts to transition the state machine from its current state to a state of the specified class.

func update(deltaTime: TimeInterval)

Tells the current state object to perform per-frame updates.

### Instance Methods

func state&lt;StateType>(forClass: StateType.Type) -> StateType?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### State Machines

class GKState

The abstract superclass for defining state-specific logic as part of a state machine.

