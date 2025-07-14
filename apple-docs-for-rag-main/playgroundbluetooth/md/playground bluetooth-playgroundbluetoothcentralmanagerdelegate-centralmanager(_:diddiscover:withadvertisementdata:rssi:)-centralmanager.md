

- Playground Bluetooth
- PlaygroundBluetoothCentralManagerDelegate
-  centralManager(\_:didDiscover:withAdvertisementData:rssi:) 

Instance Method

# centralManager(\_:didDiscover:withAdvertisementData:rssi:)

Tells the delegate that a peripheral has been discovered during scanning.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func centralManager(
    _ centralManager: PlaygroundBluetoothCentralManager,
    didDiscover peripheral: CBPeripheral,
    withAdvertisementData advertisementData: [String : Any]?,
    rssi: Double
)
```

**Required** Default implementation provided.

## Parameters 

`centralManager`  

The central manager providing this information.

`peripheral`  

The newly discovered peripheral.

`advertisementData`  

A dictionary containing any advertisement data that the peripheral provides.

`rssi`  

The current received signal strength indicator of the peripheral in decibels.

## Default Implementations

### PlaygroundBluetoothCentralManagerDelegate Implementations

func centralManager(PlaygroundBluetoothCentralManager, didDiscover: CBPeripheral, withAdvertisementData: [String : Any]?, rssi: Double)

Tells the delegate that a peripheral has been discovered during scanning.

## See Also

### Discovering Peripherals

func centralManager(PlaygroundBluetoothCentralManager, willConnectTo: CBPeripheral)

Tells the delegate that the central manager is about to attempt to establish a connection with a peripheral.

**Required** Default implementation provided.

func centralManager(PlaygroundBluetoothCentralManager, didConnectTo: CBPeripheral)

Tells the delegate that the central manager established a connection with a peripheral.

**Required** Default implementation provided.

