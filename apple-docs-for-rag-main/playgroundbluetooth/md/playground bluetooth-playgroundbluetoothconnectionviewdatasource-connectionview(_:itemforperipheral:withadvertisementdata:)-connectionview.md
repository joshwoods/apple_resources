

- Playground Bluetooth
- PlaygroundBluetoothConnectionViewDataSource
-  connectionView(\_:itemForPeripheral:withAdvertisementData:) 

Instance Method

# connectionView(\_:itemForPeripheral:withAdvertisementData:)

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connectionView(
    _ connectionView: PlaygroundBluetoothConnectionView,
    itemForPeripheral peripheral: CBPeripheral,
    withAdvertisementData advertisementData: [String : Any]?
) -> PlaygroundBluetoothConnectionView.Item
```

**Required**

## Parameters 

`connectionView`  

The connection view showing available peripherals.

`peripheral`  

The peripheral to display in the connection view.

`advertisementData`  

The advertisement data you use to help decide how to display the peripheral.

## Return Value

A PlaygroundBluetoothConnectionView.Item instance that's displayed within a PlaygroundBluetoothConnectionView.

