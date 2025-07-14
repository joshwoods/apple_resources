

- Playground Bluetooth
- PlaygroundBluetoothCentralManagerDelegate
-  centralManager(\_:didDisconnectFrom:error:) 

Instance Method

# centralManager(\_:didDisconnectFrom:error:)

Tells the delegate that the central manager disconnected from a peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func centralManager(
    _ centralManager: PlaygroundBluetoothCentralManager,
    didDisconnectFrom peripheral: CBPeripheral,
    error: Error?
)
```

**Required** Default implementation provided.

## Parameters 

`centralManager`  

The central manager that disconnected from a peripheral.

`peripheral`  

The peripheral that the central manager disconnected from.

`error`  

An error which, if present, describes the reason for the connection failure. The absence of an error indicates that the disconnection was requested via the manager’s disconnect(from:) method.

## Default Implementations

### PlaygroundBluetoothCentralManagerDelegate Implementations

func centralManager(PlaygroundBluetoothCentralManager, didDisconnectFrom: CBPeripheral, error: Error?)

Tells the delegate that the central manager disconnected from a peripheral.

## See Also

### Handling Disconnects

func centralManager(PlaygroundBluetoothCentralManager, didFailToConnectTo: CBPeripheral, error: Error?)

Tells the delegate that the central manager failed to establish a connection with a peripheral.

**Required** Default implementation provided.

