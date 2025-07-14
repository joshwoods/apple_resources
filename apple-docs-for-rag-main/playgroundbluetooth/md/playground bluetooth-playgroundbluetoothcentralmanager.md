

- Playground Bluetooth
-  PlaygroundBluetoothCentralManager 

Class

# PlaygroundBluetoothCentralManager

A streamlined interface for connecting the central manager for the current playground page to nearby Bluetooth peripherals.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
class PlaygroundBluetoothCentralManager
```

## Topics

### Configuring Central Managers

init(services: [CBUUID]?, queue: DispatchQueue)

Creates a central manager that supports communicating with Bluetooth peripherals.

var delegate: PlaygroundBluetoothCentralManagerDelegate?

A delegate that can receive messages from the central manager by adopting the PlaygroundBluetoothCentralManagerDelegate protocol.

var scanning: Bool

A Boolean value that determines whether the central manager is scanning for peripherals.

### Connecting Peripherals

func connect(to: CBPeripheral, timeout: TimeInterval?, callback: ((CBPeripheral, Error?) -> Void)?)

Attempts to connect the central manager to the specified peripheral.

func connect(toPeripheralWithUUID: UUID, timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?)

Attempts to connect the central manager to a peripheral with the specified unique identifier.

func connectToLastConnectedPeripheral(timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?) -> Bool

Attempts to reconnect the central manager to the most recently connected peripheral.

enum PlaygroundBluetoothCentralManager.ConnectionError

The errors you may encounter when connecting a peripheral to the central manager for the current playground page.

### Disconnecting Peripherals

func disconnect(from: CBPeripheral)

Disconnects the central manager from the specified, connected peripheral.

### Inspecting Central Managers

var connectedPeripherals: [CBPeripheral]

An array of the peripherals currently connected to the central manager.

var state: CBManagerState

The current state of the central manager.

## See Also

### Peripheral Connection

Connecting to Bluetooth Peripherals in Swift Playgrounds

Scan for peripherals and display them in your playground's live view.

protocol PlaygroundBluetoothCentralManagerDelegate

A delegate you use to respond to peripheral discovery and manage the lifecycle of connections.

