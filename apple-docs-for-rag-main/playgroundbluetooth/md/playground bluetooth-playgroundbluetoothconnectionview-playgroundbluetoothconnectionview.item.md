

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  PlaygroundBluetoothConnectionView.Item 

Structure

# PlaygroundBluetoothConnectionView.Item

A value that holds information about a peripheral displayed in a connection view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
struct PlaygroundBluetoothConnectionView.Item
```

## Topics

### Displaying Peripheral Information

init(name: String, icon: UIImage, issueIcon: UIImage, firmwareStatus: PlaygroundBluetoothConnectionView.Item.FirmwareStatus?, batteryLevel: Double?)

Creates a structure that holds information about a peripheral displayed in a connection view.

var name: String

The name of a peripheral as it should appear in a connection view.

### Displaying Icons

var icon: UIImage

An image that represents a peripheral.

var issueIcon: UIImage

An image indicating that a peripheral may not function correctly.

### Displaying Statuses

var batteryLevel: Double?

A value between 0 and 1.0 indicating a peripheral’s percent battery charge.

var firmwareStatus: PlaygroundBluetoothConnectionView.Item.FirmwareStatus?

A value that indicates whether a peripheral needs a firmware update.

enum PlaygroundBluetoothConnectionView.Item.FirmwareStatus

The states you use to indicate whether a peripheral’s firmware is current

## See Also

### Displaying Peripherals

func setItem(PlaygroundBluetoothConnectionView.Item, forPeripheral: CBPeripheral)

Sets all of the information about the specified peripheral at once.

