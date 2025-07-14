

- Playground Bluetooth
- PlaygroundBluetoothCentralManagerDelegate
-  centralManager(\_:didFailToConnectTo:error:) 

Instance Method

# centralManager(\_:didFailToConnectTo:error:)

Tells the delegate that the central manager failed to establish a connection with a peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func centralManager(
    _ centralManager: PlaygroundBluetoothCentralManager,
    didFailToConnectTo peripheral: CBPeripheral,
    error: Error?
)
```

**Required** Default implementation provided.

## Parameters 

`centralManager`  

The central manager that failed to make the new connection.

`peripheral`  

The peripheral that the central manager couldn’t connect to.

`error`  

An error which describes the reason for the connection failure.

## Default Implementations

### PlaygroundBluetoothCentralManagerDelegate Implementations

func centralManager(PlaygroundBluetoothCentralManager, didFailToConnectTo: CBPeripheral, error: Error?)

Tells the delegate that the central manager failed to establish a connection with a peripheral.

## See Also

### Handling Disconnects

func centralManager(PlaygroundBluetoothCentralManager, didDisconnectFrom: CBPeripheral, error: Error?)

Tells the delegate that the central manager disconnected from a peripheral.

**Required** Default implementation provided.

