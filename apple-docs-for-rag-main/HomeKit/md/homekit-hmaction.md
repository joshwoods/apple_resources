

- HomeKit
-  HMAction 

Class

# HMAction

An abstract base class for actions in HomeKit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMAction
```

## Overview

Actions can be added to HMActionSet objects. Action sets can then be set for automatic execution in response to specific conditions using HMTrigger objects, or manually triggered with executeActionSet(_:completionHandler:).

## Topics

### Identifying an action

var uniqueIdentifier: UUID

A unique identifier for the action.

### Initializers

init()Deprecated

### Type Methods

class func new() -> SelfDeprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- HMCharacteristicWriteAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Related Documentation

HomeKit Developer Guide

### Defining the associated actions

var actions: Set&lt;HMAction>

Set of actions in the action set.

func addAction(HMAction, completionHandler: HMErrorBlock)

Adds an action to the action set.

func removeAction(HMAction, completionHandler: HMErrorBlock)

Removes an action from the action set.

class HMCharacteristicWriteAction

An action in an action set that writes a value to a characteristic.

