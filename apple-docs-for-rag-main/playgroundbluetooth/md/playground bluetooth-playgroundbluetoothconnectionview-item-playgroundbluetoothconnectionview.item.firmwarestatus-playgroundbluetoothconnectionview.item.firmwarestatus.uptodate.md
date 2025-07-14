

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- Item
- PlaygroundBluetoothConnectionView.Item.FirmwareStatus
-  PlaygroundBluetoothConnectionView.Item.FirmwareStatus.upToDate 

Enumeration Case

# PlaygroundBluetoothConnectionView.Item.FirmwareStatus.upToDate

The state that indicates that a peripheral doesn’t need a firmware update.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case upToDate
```

## See Also

### Determining Firmware Status

case outOfDate

The state that indicates that a peripheral needs a firmware update before it can operate correctly.

static func != (PlaygroundBluetoothConnectionView.Item.FirmwareStatus, PlaygroundBluetoothConnectionView.Item.FirmwareStatus) -> Bool

Compares two firmware statuses and returns `true` when they're different.

