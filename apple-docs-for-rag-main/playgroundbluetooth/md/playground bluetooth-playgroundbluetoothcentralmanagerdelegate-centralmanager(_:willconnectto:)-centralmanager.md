

- Playground Bluetooth
- PlaygroundBluetoothCentralManagerDelegate
-  centralManager(\_:willConnectTo:) 

Instance Method

# centralManager(\_:willConnectTo:)

Tells the delegate that the central manager is about to attempt to establish a connection with a peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func centralManager(
    _ centralManager: PlaygroundBluetoothCentralManager,
    willConnectTo peripheral: CBPeripheral
)
```

**Required** Default implementation provided.

## Parameters 

`centralManager`  

The central manager attempting the new connection.

`peripheral`  

The peripheral that the central manager is attempting to connect to.

## Default Implementations

### PlaygroundBluetoothCentralManagerDelegate Implementations

func centralManager(PlaygroundBluetoothCentralManager, willConnectTo: CBPeripheral)

Tells the delegate that the central manager is about to attempt to establish a connection with a peripheral.

## See Also

### Discovering Peripherals

func centralManager(PlaygroundBluetoothCentralManager, didDiscover: CBPeripheral, withAdvertisementData: [String : Any]?, rssi: Double)

Tells the delegate that a peripheral has been discovered during scanning.

**Required** Default implementation provided.

func centralManager(PlaygroundBluetoothCentralManager, didConnectTo: CBPeripheral)

Tells the delegate that the central manager established a connection with a peripheral.

**Required** Default implementation provided.

