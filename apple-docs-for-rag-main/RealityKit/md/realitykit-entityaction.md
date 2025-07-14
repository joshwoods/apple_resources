

- RealityKit
-  EntityAction 

Protocol

# EntityAction

A protocol that defines an action for an entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
protocol EntityAction
```

## Overview

Structures that conform to `EntityAction` can contain data that an ActionAnimation stores. If your apps needs to serialize the animation resource to a file, the structure also needs to adopt and conform to the Codable protocol.

As action animation playback occurs, unique action events are raised for its associated `EntityAction` conforming type.

These events allow application code to animate target values (see AnimationStateProtocol), and perform custom operations in lock step with animation playback.

The action data stored within an action animation is available to the action’s event handler.

Note

Custom actions don’t support animating BlendShapeWeights.

## Topics

### Associated Types

associatedtype EventParameterType = Never

The associated event parameter type.

**Required**

### Instance Properties

var animatedValueType: (any AnimatableData.Type)?

A value that defines the type that the action animates, if the action animates a target value.

**Required**

var isAdditive: Bool

A Boolean value that determines whether this action additively blends with the prior stage.

**Required** Default implementation provided.

var isReversible: Bool

A Boolean value that determines whether the action reverses prior operations when playback is reverses.

**Required** Default implementation provided.

### Type Methods

static func registerAction()

Registers the serializable action into the action-types registry.

static func registerAction()

Registers the action into the action-types registry.

static func subscribe(to: ActionEventType, (ActionEvent&lt;Self>) -> Void)

Subscribes to a serializable action event.

static func subscribe(to: ActionEventType, (ActionEvent&lt;Self>) -> Void)

Subscribes to an action event.

static func unsubscribe(from: ActionEventType)

Unsubscribes from an action event.

static func unsubscribeAll()

Unsubscribes from all action events.

## Relationships

### Conforming Types

- BillboardAction
- EmphasizeAction
- FromToByAction
- ImpulseAction
- OrbitEntityAction
- PlayAnimationAction
- PlayAudioAction
- SetEntityEnabledAction
- SpinAction

## See Also

### Action management

struct ActionAnimation

Defines an an action animation.

enum ActionEntityResolution

Options available to determine the resolution method for a target entity in an action.

protocol ActionHandlerProtocol

The base protocol for action handlers.

