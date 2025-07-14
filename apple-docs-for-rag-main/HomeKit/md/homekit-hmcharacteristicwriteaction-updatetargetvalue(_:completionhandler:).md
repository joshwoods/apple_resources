

- HomeKit
- HMCharacteristicWriteAction
-  updateTargetValue(\_:completionHandler:) 

Instance Method

# updateTargetValue(\_:completionHandler:)

Updates the target value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func updateTargetValue(
    _ targetValue: TargetValueType,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateTargetValue(_ targetValue: TargetValueType) async throws
```

## Parameters 

`targetValue`  

The new target value.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### New Methods

init(characteristic: HMCharacteristic, targetValue: TargetValueType)

Initialize a characteristic write action with a specified characteristic and target value.

var characteristic: HMCharacteristic

The characteristic whose value is to be written by the action.

var targetValue: TargetValueType

The value that will be written to the characteristic when the action is executed.

