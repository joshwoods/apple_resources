

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- PlaygroundBluetoothConnectionView.State
-  PlaygroundBluetoothConnectionView.State.selectingPeripherals 

Enumeration Case

# PlaygroundBluetoothConnectionView.State.selectingPeripherals

One or more peripherals have been discovered and can be selected.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case selectingPeripherals
```

## Discussion

The connection view title corresponding to this state should be in one of the following formats:

&quot;Select a \(item.name)&quot;

// Or:
&quot;Select several \(item.name)s&quot;

