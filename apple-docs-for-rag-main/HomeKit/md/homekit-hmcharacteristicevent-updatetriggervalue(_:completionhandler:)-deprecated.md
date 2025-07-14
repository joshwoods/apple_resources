

- HomeKit
- HMCharacteristicEvent
-  updateTriggerValue(\_:completionHandler:) Deprecated

Instance Method

# updateTriggerValue(\_:completionHandler:)

Changes the trigger value associated with this event.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func updateTriggerValue(
    _ triggerValue: TriggerValueType?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

**Mac Catalyst, visionOS**

``` source
func updateTriggerValue(_ triggerValue: TriggerValueType?) async throws
```

Deprecated

Use the mutable region property on the HMMutableLocationEvent subclass of HMLocationEvent instead.

## Parameters 

`triggerValue`  

The value of the characteristic that triggers the event.

`completion`  

The block executed once the trigger value update request has been processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

Set the trigger value to `nil` to trigger the event whenever the value of the characteristic changes.

