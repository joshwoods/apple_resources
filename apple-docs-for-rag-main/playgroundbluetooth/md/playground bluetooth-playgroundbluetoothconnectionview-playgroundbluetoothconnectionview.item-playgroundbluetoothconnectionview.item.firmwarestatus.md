

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- PlaygroundBluetoothConnectionView.Item
-  PlaygroundBluetoothConnectionView.Item.FirmwareStatus 

Enumeration

# PlaygroundBluetoothConnectionView.Item.FirmwareStatus

The states you use to indicate whether a peripheral’s firmware is current

Xcode 10.2+Swift Playgrounds 2.0+

``` source
enum PlaygroundBluetoothConnectionView.Item.FirmwareStatus
```

## Topics

### Determining Firmware Status

case outOfDate

The state that indicates that a peripheral needs a firmware update before it can operate correctly.

case upToDate

The state that indicates that a peripheral doesn’t need a firmware update.

static func != (PlaygroundBluetoothConnectionView.Item.FirmwareStatus, PlaygroundBluetoothConnectionView.Item.FirmwareStatus) -> Bool

Compares two firmware statuses and returns `true` when they're different.

## See Also

### Displaying Statuses

var batteryLevel: Double?

A value between 0 and 1.0 indicating a peripheral’s percent battery charge.

var firmwareStatus: PlaygroundBluetoothConnectionView.Item.FirmwareStatus?

A value that indicates whether a peripheral needs a firmware update.

