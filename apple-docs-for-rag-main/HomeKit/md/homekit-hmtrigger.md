

- HomeKit
-  HMTrigger 

Class

# HMTrigger

An abstract base class for triggering actions based on a set of conditions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMTrigger
```

## Overview

This class defines the basic behavior of triggers, but does not itself specify any criteria for firing a trigger. Use instances of subclasses of HMTrigger to set up concrete triggers for actions.

## Topics

### Managing Triggers

var name: String

The name of the trigger.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the trigger.

var isEnabled: Bool

State of the trigger.

func enable(Bool, completionHandler: ((any Error)?) -> Void)

Changes the enabled state of the trigger.

var lastFireDate: Date?

The last time this trigger fired.

Deprecated

var uniqueIdentifier: UUID

A unique identifier for this trigger.

### Managing Action Sets

var actionSets: [HMActionSet]

Array of all action sets that will be executed by the trigger.

func addActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Adds an action set to the trigger.

func removeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Removes an action set from the trigger.

## Relationships

### Inherits From

- NSObject

### Inherited By

- HMEventTrigger
- HMTimerTrigger

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Triggering an action set

var triggers: [HMTrigger]

An array of triggers defined in the home.

func addTrigger(HMTrigger, completionHandler: ((any Error)?) -> Void)

Adds a trigger to the home.

func removeTrigger(HMTrigger, completionHandler: ((any Error)?) -> Void)

Removes a trigger from the home.

class HMTimerTrigger

A trigger to activate an action set based on a periodic timer.

class HMEventTrigger

A trigger to activate an action set based on a set of events and optional conditions.

