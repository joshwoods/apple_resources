

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- PlaygroundBluetoothConnectionView.State
-  PlaygroundBluetoothConnectionView.State.connecting 

Enumeration Case

# PlaygroundBluetoothConnectionView.State.connecting

The peripheral is in the process of connecting to a connection view’s central manager.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case connecting
```

## Discussion

The connection view title corresponding to this state should be in the following format:

&quot;Connecting \(item.name)&quot;

## See Also

### Waiting for Connections

case noConnection

The connection to a peripheral has been lost.

case searchingForPeripherals

A connection view’s central manager is scanning for nearby peripherals.

