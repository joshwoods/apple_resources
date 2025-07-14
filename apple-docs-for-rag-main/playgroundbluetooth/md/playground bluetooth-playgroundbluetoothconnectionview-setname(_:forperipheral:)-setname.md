

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  setName(\_:forPeripheral:) 

Instance Method

# setName(\_:forPeripheral:)

Displays the name of the specified peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func setName(
    _ name: String,
    forPeripheral peripheral: CBPeripheral
)
```

## Parameters 

`name`  

The user-facing name of the specified peripheral.

`peripheral`  

The peripheral corresponding to the name.

## See Also

### Displaying Individual Details

func setBatteryLevel(Double?, forPeripheral: CBPeripheral)

Displays the battery level for the specified peripheral.

func setFirmwareStatus(PlaygroundBluetoothConnectionView.Item.FirmwareStatus?, forPeripheral: CBPeripheral)

Displays whether or not the specified peripheral’s firmware is up-to-date.

func setIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon representing the specified peripheral.

func setIssueIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon indicating that the specified peripheral is available but may not be usable.

