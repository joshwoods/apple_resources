

- HomeKit
-  HMPresenceKeyPath 

Global Variable

# HMPresenceKeyPath

Specifies the key path for a presence event in a predicate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let HMPresenceKeyPath: String
```

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

class func predicateForEvaluatingTrigger(HMCharacteristic, relatedBy: NSComparisonPredicate.Operator, toValue: Any) -> NSPredicate

Creates a predicate that evaluates whether a characteristic value relates to the specified value.

class func predicateForEvaluatingTrigger(withPresence: HMPresenceEvent) -> NSPredicate

Creates a predicate that evaluates the current user presence against that specified in the presence event.

let HMCharacteristicKeyPath: String

Specifies the key path for a characteristic in a predicate.

let HMCharacteristicValueKeyPath: String

Specifies the key path for a characteristic value in a predicate.

