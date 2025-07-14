

- HomeKit
-  HMEventTrigger 

Class

# HMEventTrigger

A trigger to activate an action set based on a set of events and optional conditions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMEventTrigger
```

## Overview

Use an HMEventTrigger object to trigger the execution of a scene when a combination of characteristic or location events and conditions occur. To create an event trigger, first create one or more event objects that fire an event when the specified trigger values are met. For example, you might create an HMCharacteristicEvent that fires when the front door is open. Then, you can use HMEventTrigger convenience methods to create optional predicates that specify conditions that must be met before a scene is executed. For example, you might create a condition that ensures the scene is executed only after sunset.

## Topics

### Creating an event trigger

init(name: String, events: [HMEvent], predicate: NSPredicate?)

Creates a new event trigger with the specified name, events, and predicate.

init(name: String, events: [HMEvent], end: [HMEvent]?, recurrences: [DateComponents]?, predicate: NSPredicate?)

Creates a new event trigger with the specified name, events, end events, recurrences, and predicate.

### Querying trigger activation state

var triggerActivationState: HMEventTriggerActivationState

The current activation state of the trigger.

enum HMEventTriggerActivationState

The activation state of an event trigger.

### Setting trigger events

var events: [HMEvent]

The events that activate the trigger.

func updateEvents([HMEvent], completionHandler: ((any Error)?) -> Void)

Updates the set of trigger events.

Location events

Events that represent the user’s movement among regions.

Time events

Events based on time, significant occurrences, and time durations.

Characteristic events

Events based on the capabilities or characteristics of accessories.

Presence events

Events based on the user’s presence in a home.

class HMEvent

The abstract base class for a HomeKit event.

### Restoring the previous scene after an event

var endEvents: [HMEvent]

The events associated with the end of scene represented by this trigger.

func updateEndEvents([HMEvent], completionHandler: ((any Error)?) -> Void)

Updates the set of end events associated with the event trigger.

### Controlling recurrence

var recurrences: [DateComponents]?

Specifies the days on which the trigger can execute.

func updateRecurrences([DateComponents]?, completionHandler: ((any Error)?) -> Void)

Updates the days of the week the trigger can repeat.

var executeOnce: Bool

A Boolean that can execute the trigger many times.

func updateExecuteOnce(Bool, completionHandler: ((any Error)?) -> Void)

Updates the repetition status of the event trigger.

### Adding a trigger condition

var predicate: NSPredicate?

The predicate to evaluate before executing the scene associated with the event trigger.

func updatePredicate(NSPredicate?, completionHandler: ((any Error)?) -> Void)

Replaces the predicate used to evaluate execution of the scene associated with the event trigger.

### Creating predicates

class func predicateForEvaluatingTriggerOccurring(beforeSignificantEvent: HMSignificantTimeEvent) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before a significant event.

class func predicateForEvaluatingTriggerOccurring(afterSignificantEvent: HMSignificantTimeEvent) -> NSPredicate

Creates a predicate that evaluates whether the event occurred after a significant event.

class func predicate(forEvaluatingTriggerOccurringBetweenSignificantEvent: HMSignificantTimeEvent, secondSignificantEvent: HMSignificantTimeEvent) -> NSPredicate

Creates a predicate that evaluates whether the event occurred between two significant events.

class func predicateForEvaluatingTrigger(occurringBefore: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before the specified time.

class func predicateForEvaluatingTrigger(occurringOn: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred at the specified time.

class func predicateForEvaluatingTrigger(occurringAfter: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred at or after the specified time.

class func predicateForEvaluatingTriggerOccurringBetweenDate(with: DateComponents, secondDateWith: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred between the specified times.

class func predicateForEvaluatingTrigger(HMCharacteristic, relatedBy: NSComparisonPredicate.Operator, toValue: Any) -> NSPredicate

Creates a predicate that evaluates whether a characteristic value relates to the specified value.

class func predicateForEvaluatingTrigger(withPresence: HMPresenceEvent) -> NSPredicate

Creates a predicate that evaluates the current user presence against that specified in the presence event.

let HMCharacteristicKeyPath: String

Specifies the key path for a characteristic in a predicate.

let HMCharacteristicValueKeyPath: String

Specifies the key path for a characteristic value in a predicate.

let HMPresenceKeyPath: String

Specifies the key path for a presence event in a predicate.

### Deprecated symbols

func addEvent(HMEvent, completionHandler: ((any Error)?) -> Void)

Adds a new event to the event trigger.

Deprecated

func removeEvent(HMEvent, completionHandler: ((any Error)?) -> Void)

Removes the specified event from the event trigger.

Deprecated

class func predicateForEvaluatingTrigger(occurringBefore: String, applyingOffset: DateComponents?) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before a significant event.

Deprecated

class func predicateForEvaluatingTrigger(occurringAfter: String, applyingOffset: DateComponents?) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before a significant event.

Deprecated

## Relationships

### Inherits From

- HMTrigger

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

class HMActionSet

A collection of actions that you trigger as a group.

class HMTimerTrigger

A trigger to activate an action set based on a periodic timer.

