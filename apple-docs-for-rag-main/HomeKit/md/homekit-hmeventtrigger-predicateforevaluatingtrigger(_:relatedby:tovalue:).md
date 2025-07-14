

- HomeKit
- HMEventTrigger
-  predicateForEvaluatingTrigger(\_:relatedBy:toValue:) 

Type Method

# predicateForEvaluatingTrigger(\_:relatedBy:toValue:)

Creates a predicate that evaluates whether a characteristic value relates to the specified value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForEvaluatingTrigger(
    _ characteristic: HMCharacteristic,
    relatedBy operatorType: NSComparisonPredicate.Operator,
    toValue value: Any
) -> NSPredicate
```

## Parameters 

`characteristic`  

The characteristic that is part of the predicate.

`operatorType`  

The relationship between the characteristic and the target value. Valid values can be Less Than, Greater Than, Less Than or Equal, Greater Than or Equal, Equal, or Not Equal. All other values cause an exception to be thrown.

`value`  

The value of the characteristic to compare when evaluating the predicate.

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

class func predicateForEvaluatingTrigger(occurringBefore: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before the specified time.

class func predicateForEvaluatingTrigger(occurringOn: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred at the specified time.

class func predicateForEvaluatingTrigger(occurringAfter: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred at or after the specified time.

class func predicateForEvaluatingTriggerOccurringBetweenDate(with: DateComponents, secondDateWith: DateComponents) -> NSPredicate

Creates a predicate that evaluates whether the event occurred between the specified times.

class func predicateForEvaluatingTrigger(withPresence: HMPresenceEvent) -> NSPredicate

Creates a predicate that evaluates the current user presence against that specified in the presence event.

let HMCharacteristicKeyPath: String

Specifies the key path for a characteristic in a predicate.

let HMCharacteristicValueKeyPath: String

Specifies the key path for a characteristic value in a predicate.

let HMPresenceKeyPath: String

Specifies the key path for a presence event in a predicate.

