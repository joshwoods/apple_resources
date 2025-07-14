

- Playground Bluetooth
- PlaygroundBluetoothConnectionViewDelegate
-  connectionView(\_:shouldDisplayDiscovered:withAdvertisementData:rssi:) 

Instance Method

# connectionView(\_:shouldDisplayDiscovered:withAdvertisementData:rssi:)

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connectionView(
    _ connectionView: PlaygroundBluetoothConnectionView,
    shouldDisplayDiscovered peripheral: CBPeripheral,
    withAdvertisementData advertisementData: [String : Any]?,
    rssi: Double
) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`connectionView`  

The connection view showing available peripherals.

`peripheral`  

The newly discovered peripheral.

`advertisementData`  

The advertisement data you use to help decide whether or not to display the peripheral.

`rssi`  

The current received signal strength indicator of the peripheral in decibels.

## Return Value

A Boolean value indicating whether the newly discovered peripheral should show up in the connection view.

## Default Implementations

### PlaygroundBluetoothConnectionViewDelegate Implementations

func connectionView(PlaygroundBluetoothConnectionView, shouldDisplayDiscovered: CBPeripheral, withAdvertisementData: [String : Any]?, rssi: Double) -> Bool

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

## See Also

### Displaying New Peripherals

func connectionView(PlaygroundBluetoothConnectionView, shouldConnectTo: CBPeripheral, withAdvertisementData: [String : Any]?) -> Bool

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

**Required** Default implementation provided.

func connectionView(PlaygroundBluetoothConnectionView, titleFor: PlaygroundBluetoothConnectionView.State) -> String

Tells the delegate that the connection view needs a title to display for its current state.

**Required**

