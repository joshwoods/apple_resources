

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
-  scanning 

Instance Property

# scanning

A Boolean value that determines whether the central manager is scanning for peripherals.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
var scanning: Bool { get set }
```

## Discussion

Set this property to `true` to start scanning for peripherals. Upon discovering a peripheral, the central manager calls the delegate’s centralManager(_:didDiscover:withAdvertisementData:rssi:) method.

## See Also

### Configuring Central Managers

init(services: [CBUUID]?, queue: DispatchQueue)

Creates a central manager that supports communicating with Bluetooth peripherals.

var delegate: PlaygroundBluetoothCentralManagerDelegate?

A delegate that can receive messages from the central manager by adopting the PlaygroundBluetoothCentralManagerDelegate protocol.

