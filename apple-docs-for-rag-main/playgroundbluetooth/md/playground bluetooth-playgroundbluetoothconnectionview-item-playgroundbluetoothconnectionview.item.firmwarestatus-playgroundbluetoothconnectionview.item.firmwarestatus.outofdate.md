

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- Item
- PlaygroundBluetoothConnectionView.Item.FirmwareStatus
-  PlaygroundBluetoothConnectionView.Item.FirmwareStatus.outOfDate 

Enumeration Case

# PlaygroundBluetoothConnectionView.Item.FirmwareStatus.outOfDate

The state that indicates that a peripheral needs a firmware update before it can operate correctly.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case outOfDate
```

## See Also

### Determining Firmware Status

case upToDate

The state that indicates that a peripheral doesn’t need a firmware update.

static func != (PlaygroundBluetoothConnectionView.Item.FirmwareStatus, PlaygroundBluetoothConnectionView.Item.FirmwareStatus) -> Bool

Compares two firmware statuses and returns `true` when they're different.

