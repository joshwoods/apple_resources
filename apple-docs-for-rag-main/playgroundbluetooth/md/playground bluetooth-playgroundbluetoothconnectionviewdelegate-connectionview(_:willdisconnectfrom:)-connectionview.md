

- Playground Bluetooth
- PlaygroundBluetoothConnectionViewDelegate
-  connectionView(\_:willDisconnectFrom:) 

Instance Method

# connectionView(\_:willDisconnectFrom:)

Tells the delegate that a connected peripheral is about to be disconnected.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connectionView(
    _ connectionView: PlaygroundBluetoothConnectionView,
    willDisconnectFrom peripheral: CBPeripheral
)
```

**Required** Default implementation provided.

## Parameters 

`connectionView`  

The connection view currently displaying the connection to this peripheral.

`peripheral`  

The peripheral facing emminent disconnection.

## Default Implementations

### PlaygroundBluetoothConnectionViewDelegate Implementations

func connectionView(PlaygroundBluetoothConnectionView, willDisconnectFrom: CBPeripheral)

Tells the delegate that a connected peripheral is about to be disconnected.

