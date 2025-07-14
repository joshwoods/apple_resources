

- HomeKit
- HMEventTrigger
-  predicateForEvaluatingTrigger(occurringBefore:applyingOffset:) Deprecated

Type Method

# predicateForEvaluatingTrigger(occurringBefore:applyingOffset:)

Creates a predicate that evaluates whether the event occurred before a significant event.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.0Deprecated

``` source
class func predicateForEvaluatingTrigger(
    occurringBefore significantEvent: String,
    applyingOffset offset: DateComponents?
) -> NSPredicate
```

Deprecated

Use predicateForEvaluatingTriggerOccurring(beforeSignificantEvent:) instead.

## Parameters 

`significantEvent`  

The significant event to compare against. Valid values for this parameter are `HMSignificantEventSunrise` and `HMSignificantEventSunset`.

`offset`  

An offset from the time of the significant event. To specify an offset before a significant event, the properties of the NSDateComponents object must be negative values. For example, to specify 30 minutes before sunset, set the minute property to `-30`.

## Return Value

A predicate object that represents a condition to evaluate before executing the scene.

## See Also

### Deprecated symbols

func addEvent(HMEvent, completionHandler: ((any Error)?) -> Void)

Adds a new event to the event trigger.

Deprecated

func removeEvent(HMEvent, completionHandler: ((any Error)?) -> Void)

Removes the specified event from the event trigger.

Deprecated

class func predicateForEvaluatingTrigger(occurringAfter: String, applyingOffset: DateComponents?) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before a significant event.

Deprecated

