

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
-  delegate 

Instance Property

# delegate

A delegate that can receive messages from the central manager by adopting the PlaygroundBluetoothCentralManagerDelegate protocol.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
weak var delegate: PlaygroundBluetoothCentralManagerDelegate?
```

## See Also

### Configuring Central Managers

init(services: [CBUUID]?, queue: DispatchQueue)

Creates a central manager that supports communicating with Bluetooth peripherals.

var scanning: Bool

A Boolean value that determines whether the central manager is scanning for peripherals.

