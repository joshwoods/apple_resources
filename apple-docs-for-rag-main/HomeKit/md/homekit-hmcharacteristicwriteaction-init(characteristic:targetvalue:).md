

- HomeKit
- HMCharacteristicWriteAction
-  init(characteristic:targetValue:) 

Initializer

# init(characteristic:targetValue:)

Initialize a characteristic write action with a specified characteristic and target value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
init(
    characteristic: HMCharacteristic,
    targetValue: TargetValueType
)
```

## Parameters 

`characteristic`  

The characteristic.

`targetValue`  

The target value for the characteristic.

## Return Value

A newly initialized characteristic write action object with the specified characteristic and target value.

## See Also

### Related Documentation

HomeKit Developer Guide

### New Methods

var characteristic: HMCharacteristic

The characteristic whose value is to be written by the action.

var targetValue: TargetValueType

The value that will be written to the characteristic when the action is executed.

func updateTargetValue(TargetValueType, completionHandler: ((any Error)?) -> Void)

Updates the target value.

