

- Accessibility
- AXMFiHearingDevice
-  pairedDeviceIdentifiers() 

Type Method

# pairedDeviceIdentifiers()

Returns the UUIDs of the hearing device peripherals.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func pairedDeviceIdentifiers() -> [UUID]
```

## Return Value

An array of UUID objects that represent the Core Bluetooth UUIDs of the hearing device peripherals.

## Discussion

This function returns each CBPeripheral with a manufacturer that matches the manufacturer in your app’s `hearing.aid.app` entitlement. For bimodal hearing devices, specify an array of manufacturers for this entitlement.

Find and connect to the matching hearing device peripherals like this:

```
let uuids = AXMFiHearingDevice.pairedDeviceIdentifiers()
let peripherals = bluetoothManager.retrievePeripherals(withIdentifiers: uuids)
for peripheral in peripherals where peripheral.state == .connected {
    bluetoothManager.connect(peripheral)
}
```

## See Also

### Paired hearing devices

static let pairedUUIDsDidChangeNotification: NSNotification.Name

A notification that the system posts when there’s a change to the UUIDs of the hearing device peripherals.

