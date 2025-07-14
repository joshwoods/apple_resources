

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  setBatteryLevel(\_:forPeripheral:) 

Instance Method

# setBatteryLevel(\_:forPeripheral:)

Displays the battery level for the specified peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func setBatteryLevel(
    _ batteryLevel: Double?,
    forPeripheral peripheral: CBPeripheral
)
```

## Parameters 

`batteryLevel`  

A value between 0 and 1.0 indicating the peripheral’s percent battery charge.

`peripheral`  

The peripheral corresponding to the battery level being displayed.

## See Also

### Displaying Individual Details

func setFirmwareStatus(PlaygroundBluetoothConnectionView.Item.FirmwareStatus?, forPeripheral: CBPeripheral)

Displays whether or not the specified peripheral’s firmware is up-to-date.

func setIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon representing the specified peripheral.

func setIssueIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon indicating that the specified peripheral is available but may not be usable.

func setName(String, forPeripheral: CBPeripheral)

Displays the name of the specified peripheral.

