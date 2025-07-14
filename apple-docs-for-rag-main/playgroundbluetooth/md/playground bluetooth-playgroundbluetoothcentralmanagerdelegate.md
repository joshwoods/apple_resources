

- Playground Bluetooth
-  PlaygroundBluetoothCentralManagerDelegate 

Protocol

# PlaygroundBluetoothCentralManagerDelegate

A delegate you use to respond to peripheral discovery and manage the lifecycle of connections.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
protocol PlaygroundBluetoothCentralManagerDelegate : AnyObject
```

## Topics

### Discovering Peripherals

func centralManager(PlaygroundBluetoothCentralManager, didDiscover: CBPeripheral, withAdvertisementData: [String : Any]?, rssi: Double)

Tells the delegate that a peripheral has been discovered during scanning.

**Required** Default implementation provided.

func centralManager(PlaygroundBluetoothCentralManager, willConnectTo: CBPeripheral)

Tells the delegate that the central manager is about to attempt to establish a connection with a peripheral.

**Required** Default implementation provided.

func centralManager(PlaygroundBluetoothCentralManager, didConnectTo: CBPeripheral)

Tells the delegate that the central manager established a connection with a peripheral.

**Required** Default implementation provided.

### Handling State Changes

func centralManagerStateDidChange(PlaygroundBluetoothCentralManager)

Tells the delegate that the state of the central manager has changed.

**Required** Default implementation provided.

### Handling Disconnects

func centralManager(PlaygroundBluetoothCentralManager, didDisconnectFrom: CBPeripheral, error: Error?)

Tells the delegate that the central manager disconnected from a peripheral.

**Required** Default implementation provided.

func centralManager(PlaygroundBluetoothCentralManager, didFailToConnectTo: CBPeripheral, error: Error?)

Tells the delegate that the central manager failed to establish a connection with a peripheral.

**Required** Default implementation provided.

## See Also

### Peripheral Connection

Connecting to Bluetooth Peripherals in Swift Playgrounds

Scan for peripherals and display them in your playground's live view.

class PlaygroundBluetoothCentralManager

A streamlined interface for connecting the central manager for the current playground page to nearby Bluetooth peripherals.

