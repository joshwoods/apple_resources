

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- PlaygroundBluetoothConnectionView.State
-  PlaygroundBluetoothConnectionView.State.searchingForPeripherals 

Enumeration Case

# PlaygroundBluetoothConnectionView.State.searchingForPeripherals

A connection view’s central manager is scanning for nearby peripherals.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case searchingForPeripherals
```

## Discussion

The connection view title corresponding to this state should be in one of the following formats:

&quot;Searching for \(item.name)&quot;

// Or:
&quot;Searching for \(item.name)s&quot;

## See Also

### Waiting for Connections

case connecting

The peripheral is in the process of connecting to a connection view’s central manager.

case noConnection

The connection to a peripheral has been lost.

