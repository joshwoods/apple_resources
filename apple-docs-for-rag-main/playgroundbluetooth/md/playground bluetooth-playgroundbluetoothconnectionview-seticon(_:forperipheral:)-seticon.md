

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  setIcon(\_:forPeripheral:) 

Instance Method

# setIcon(\_:forPeripheral:)

Displays an icon representing the specified peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func setIcon(
    _ icon: UIImage,
    forPeripheral peripheral: CBPeripheral
)
```

## Parameters 

`icon`  

An icon that represents the specified peripheral.

`peripheral`  

The peripheral corresponding to the icon being displayed.

## See Also

### Displaying Individual Details

func setBatteryLevel(Double?, forPeripheral: CBPeripheral)

Displays the battery level for the specified peripheral.

func setFirmwareStatus(PlaygroundBluetoothConnectionView.Item.FirmwareStatus?, forPeripheral: CBPeripheral)

Displays whether or not the specified peripheral’s firmware is up-to-date.

func setIssueIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon indicating that the specified peripheral is available but may not be usable.

func setName(String, forPeripheral: CBPeripheral)

Displays the name of the specified peripheral.

