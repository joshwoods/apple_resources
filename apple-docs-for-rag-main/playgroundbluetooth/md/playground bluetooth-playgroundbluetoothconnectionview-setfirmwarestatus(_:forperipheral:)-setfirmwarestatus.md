

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  setFirmwareStatus(\_:forPeripheral:) 

Instance Method

# setFirmwareStatus(\_:forPeripheral:)

Displays whether or not the specified peripheral’s firmware is up-to-date.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func setFirmwareStatus(
    _ firmwareStatus: PlaygroundBluetoothConnectionView.Item.FirmwareStatus?,
    forPeripheral peripheral: CBPeripheral
)
```

## Parameters 

`firmwareStatus`  

A value that indicates whether the specified peripheral needs a firmware update.

`peripheral`  

The peripheral corresponding to the firmware readiness being set.

## See Also

### Displaying Individual Details

func setBatteryLevel(Double?, forPeripheral: CBPeripheral)

Displays the battery level for the specified peripheral.

func setIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon representing the specified peripheral.

func setIssueIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon indicating that the specified peripheral is available but may not be usable.

func setName(String, forPeripheral: CBPeripheral)

Displays the name of the specified peripheral.

