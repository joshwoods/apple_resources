

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- PlaygroundBluetoothConnectionView.State
-  PlaygroundBluetoothConnectionView.State.noConnection 

Enumeration Case

# PlaygroundBluetoothConnectionView.State.noConnection

The connection to a peripheral has been lost.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case noConnection
```

## Discussion

The connection view title corresponding to this state should be in the following format:

&quot;Connect \(item.name)&quot;

## See Also

### Waiting for Connections

case connecting

The peripheral is in the process of connecting to a connection view’s central manager.

case searchingForPeripherals

A connection view’s central manager is scanning for nearby peripherals.

