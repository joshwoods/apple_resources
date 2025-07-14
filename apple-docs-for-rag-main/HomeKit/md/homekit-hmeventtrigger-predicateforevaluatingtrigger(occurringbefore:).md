

- HomeKit
- HMEventTrigger
-  predicateForEvaluatingTrigger(occurringBefore:) 

Type Method

# predicateForEvaluatingTrigger(occurringBefore:)

Creates a predicate that evaluates whether the event occurred before the specified time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForEvaluatingTrigger(occurringBefore dateComponents: DateComponents) -> NSPredicate
```

## Parameters 

`dateComponents`  

Date components that represent the time to compare with the time that the event occurred.

## Return Value

A predicate object that represents a condition to evaluate before executing the scene.

## See Also

### Creating predicates

class func predicateForEvaluatingTriggerOccurring(beforeSignificantEvent: HMSignificantTimeEvent) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before a significant event.

class func predicateForEvaluatingTriggerOccurring(afterSignificantEvent: HMSignificantTimeEvent) -> NSPredicate

Creates a predicate that evaluates whether the event occurred after a significant event.

class func predicate(forEvaluatingTriggerOccurringBetweenSignificantEvent: HMSignificantTimeEvent, secondSignificantEvent: HMSignificantTimeEvent) -> NSPredicate

Creates a predicate that evaluates whether the event occurred between two significant events.

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

