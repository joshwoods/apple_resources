

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- PlaygroundBluetoothConnectionView.Item
- PlaygroundBluetoothConnectionView.Item.FirmwareStatus
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Compares two firmware statuses and returns `true` when they're different.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
static func != (lhs: PlaygroundBluetoothConnectionView.Item.FirmwareStatus, rhs: PlaygroundBluetoothConnectionView.Item.FirmwareStatus) -> Bool
```

## See Also

### Determining Firmware Status

case outOfDate

The state that indicates that a peripheral needs a firmware update before it can operate correctly.

case upToDate

The state that indicates that a peripheral doesn’t need a firmware update.

