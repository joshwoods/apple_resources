

- Playground Bluetooth
-  PlaygroundBluetoothConnectionViewDelegate 

Protocol

# PlaygroundBluetoothConnectionViewDelegate

A delegate you use to respond to user- and system-initiated interactions with the central manager’s connection view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
protocol PlaygroundBluetoothConnectionViewDelegate : AnyObject
```

## Topics

### Displaying New Peripherals

func connectionView(PlaygroundBluetoothConnectionView, shouldConnectTo: CBPeripheral, withAdvertisementData: [String : Any]?) -> Bool

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

**Required** Default implementation provided.

func connectionView(PlaygroundBluetoothConnectionView, shouldDisplayDiscovered: CBPeripheral, withAdvertisementData: [String : Any]?, rssi: Double) -> Bool

Tells the delegate that a new peripheral was discovered and can be displayed in the connection view.

**Required** Default implementation provided.

func connectionView(PlaygroundBluetoothConnectionView, titleFor: PlaygroundBluetoothConnectionView.State) -> String

Tells the delegate that the connection view needs a title to display for its current state.

**Required**

### Displaying Firmware Update Information

func connectionView(PlaygroundBluetoothConnectionView, firmwareUpdateInstructionsFor: CBPeripheral) -> String

Tells the delegate that a peripheral has a firmware update available.

**Required**

### Disconnecting from Peripherals

func connectionView(PlaygroundBluetoothConnectionView, willDisconnectFrom: CBPeripheral)

Tells the delegate that a connected peripheral is about to be disconnected.

**Required** Default implementation provided.

## See Also

### Peripheral Display

class PlaygroundBluetoothConnectionView

A view that displays the connection status of a peripheral to the central manager for the current page and manages connections to other peripherals.

protocol PlaygroundBluetoothConnectionViewDataSource

The protocol you adopt to display an available peripheral in a playground page’s connection view.

