

- Playground Bluetooth
- PlaygroundBluetoothConnectionViewDelegate
-  connectionView(\_:titleFor:) 

Instance Method

# connectionView(\_:titleFor:)

Tells the delegate that the connection view needs a title to display for its current state.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connectionView(
    _ connectionView: PlaygroundBluetoothConnectionView,
    titleFor state: PlaygroundBluetoothConnectionView.State
) -> String
```

**Required**

## Parameters 

`connectionView`  

The connection view that’s entering this state.

`state`  

The state of the view. The state is one of the cases of the PlaygroundBluetoothConnectionView.State enumeration.

## Return Value

A localized string corresponding to the current state of the view.

## See Also

### Displaying New Peripherals

func connectionView(PlaygroundBluetoothConnectionView, shouldConnectTo: CBPeripheral, withAdvertisementData: [String : Any]?) -> Bool

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

**Required** Default implementation provided.

func connectionView(PlaygroundBluetoothConnectionView, shouldDisplayDiscovered: CBPeripheral, withAdvertisementData: [String : Any]?, rssi: Double) -> Bool

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

**Required** Default implementation provided.

