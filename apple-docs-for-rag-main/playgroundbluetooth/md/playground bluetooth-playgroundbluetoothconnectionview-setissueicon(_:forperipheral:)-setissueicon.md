

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  setIssueIcon(\_:forPeripheral:) 

Instance Method

# setIssueIcon(\_:forPeripheral:)

Displays an icon indicating that the specified peripheral is available but may not be usable.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func setIssueIcon(
    _ issueIcon: UIImage,
    forPeripheral peripheral: CBPeripheral
)
```

## Parameters 

`issueIcon`  

An icon indicating that the specified peripheral may not function correctly.

`peripheral`  

The problematic peripheral.

## Discussion

Use an issue icon to indicate problems such as outdated firmware or a lost connection.

## See Also

### Displaying Individual Details

func setBatteryLevel(Double?, forPeripheral: CBPeripheral)

Displays the battery level for the specified peripheral.

func setFirmwareStatus(PlaygroundBluetoothConnectionView.Item.FirmwareStatus?, forPeripheral: CBPeripheral)

Displays whether or not the specified peripheral’s firmware is up-to-date.

func setIcon(UIImage, forPeripheral: CBPeripheral)

Displays an icon representing the specified peripheral.

func setName(String, forPeripheral: CBPeripheral)

Displays the name of the specified peripheral.

