

- HomeKit
- HMEventTrigger
-  removeEvent(\_:completionHandler:) Deprecated

Instance Method

# removeEvent(\_:completionHandler:)

Removes the specified event from the event trigger.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func removeEvent(
    _ event: HMEvent,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

**Mac Catalyst, visionOS**

``` source
func removeEvent(_ event: HMEvent) async throws
```

Deprecated

Use updateEvents(_:completionHandler:) instead.

## Parameters 

`event`  

The event to remove from the event trigger.

`completion`  

A block that executes after processing the request.

The block takes the following parameter:

error  
If the request was successful, the value of `error` is `nil`; otherwise, the value provides more information about the request status.

## See Also

### Deprecated symbols

func addEvent(HMEvent, completionHandler: ((any Error)?) -> Void)

Adds a new event to the event trigger.

Deprecated

class func predicateForEvaluatingTrigger(occurringBefore: String, applyingOffset: DateComponents?) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before a significant event.

Deprecated

class func predicateForEvaluatingTrigger(occurringAfter: String, applyingOffset: DateComponents?) -> NSPredicate

Creates a predicate that evaluates whether the event occurred before a significant event.

Deprecated

