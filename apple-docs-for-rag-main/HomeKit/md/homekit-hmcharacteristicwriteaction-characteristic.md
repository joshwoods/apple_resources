

- HomeKit
- HMCharacteristicWriteAction
-  characteristic 

Instance Property

# characteristic

The characteristic whose value is to be written by the action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var characteristic: HMCharacteristic { get }
```

## See Also

### New Methods

init(characteristic: HMCharacteristic, targetValue: TargetValueType)

Initialize a characteristic write action with a specified characteristic and target value.

var targetValue: TargetValueType

The value that will be written to the characteristic when the action is executed.

func updateTargetValue(TargetValueType, completionHandler: ((any Error)?) -> Void)

Updates the target value.

