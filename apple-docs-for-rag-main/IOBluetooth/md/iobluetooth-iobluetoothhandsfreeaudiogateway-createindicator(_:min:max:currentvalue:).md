

- IOBluetooth
- IOBluetoothHandsFreeAudioGateway
-  createIndicator(\_:min:max:currentValue:) 

Instance Method

# createIndicator(\_:min:max:currentValue:)

Sends a request to the Bluetooth device to show or update a status indicator.

macOS 10.7+

``` source
func createIndicator(
    _ indicatorName: String!,
    min minValue: Int32,
    max maxValue: Int32,
    currentValue: Int32
)
```

## Parameters 

`indicatorName`  

The name of the indicator. Use one of the following constants:

- IOBluetoothHandsFreeIndicatorService

- IOBluetoothHandsFreeIndicatorCall

- IOBluetoothHandsFreeIndicatorCallSetup

- IOBluetoothHandsFreeIndicatorCallHeld

- IOBluetoothHandsFreeIndicatorSignal

- IOBluetoothHandsFreeIndicatorRoam

- IOBluetoothHandsFreeIndicatorBattChg

`minValue`  

The minimum value for the indicator.

`maxValue`  

The maximum value for the indicator.

`currentValue`  

The current value of the indicator.

## See Also

### Showing Status Indicators

Status Indicator Constants

Send commands to modify the status indicators of a hands-free Bluetooth device.

