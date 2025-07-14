

- HomeKit
- HMCharacteristicEvent
-  init(characteristic:triggerValue:) 

Initializer

# init(characteristic:triggerValue:)

Creates a new characteristic event which triggers when the specified characteristic reaches the specified value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+

``` source
init(
    characteristic: HMCharacteristic,
    triggerValue: TriggerValueType?
)
```

## Parameters 

`characteristic`  

The characteristic that the event is observing.

`triggerValue`  

The value of the characteristic that triggers the event. Specifying `nil` causes the event to fire every time the value of the characteristic changes.

## Return Value

An initialized characteristic event for the specified characteristic and trigger value.

## Discussion

Use a characteristic that supports notification; otherwise this initializer throws an exception.

