

- HomeKit
-  HMActionSet 

Class

# HMActionSet

A collection of actions that you trigger as a group.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMActionSet
```

## Overview

Action sets can be executed as a result of evaluating a trigger (instances of HMTrigger) or manually with executeActionSet(_:completionHandler:). Actions in an action set are performed in an unspecified order. You create new action sets using the addActionSet(withName:completionHandler:) method of HMHome.

## Topics

### Identifiying an action set

var uniqueIdentifier: UUID

The action set’s unique identifier.

var name: String

The name of the action set.

func updateName(String, completionHandler: HMErrorBlock)

Updates the name of the action set.

### Specifying a type

var actionSetType: String

The type of the action set, such as built-in or user-defined.

Action Set Types

The types of action sets that you can define.

### Defining the associated actions

var actions: Set&lt;HMAction>

Set of actions in the action set.

func addAction(HMAction, completionHandler: HMErrorBlock)

Adds an action to the action set.

func removeAction(HMAction, completionHandler: HMErrorBlock)

Removes an action from the action set.

class HMCharacteristicWriteAction

An action in an action set that writes a value to a characteristic.

class HMAction

An abstract base class for actions in HomeKit.

### Keeping track of execution

var isExecuting: Bool

The execution status of the action set.

var lastExecutionDate: Date?

The last execution date of the action set.

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
- Sendable

## See Also

### Action Sets

class HMTimerTrigger

A trigger to activate an action set based on a periodic timer.

class HMEventTrigger

A trigger to activate an action set based on a set of events and optional conditions.

