

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
-  init(services:queue:) 

Initializer

# init(services:queue:)

Creates a central manager that supports communicating with Bluetooth peripherals.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
init(
    services: [CBUUID]?,
    queue: DispatchQueue = .main
)
```

## Parameters 

`services`  

An array of service identifiers that the central manager scans for. If `nil`, all peripherals in range are eligible for connection attempts.

`queue`  

The dispatch queue used to dispatch events to the central manager’s delegate.

## See Also

### Configuring Central Managers

var delegate: PlaygroundBluetoothCentralManagerDelegate?

A delegate that can receive messages from the central manager by adopting the PlaygroundBluetoothCentralManagerDelegate protocol.

var scanning: Bool

A Boolean value that determines whether the central manager is scanning for peripherals.

