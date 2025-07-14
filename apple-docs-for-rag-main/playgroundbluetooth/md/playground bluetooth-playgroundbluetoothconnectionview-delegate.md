

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  delegate 

Instance Property

# delegate

A delegate you supply to make decisions about which peripherals are displayed in the view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
weak var delegate: PlaygroundBluetoothConnectionViewDelegate? { get set }
```

## See Also

### Handling State Changes

enum PlaygroundBluetoothConnectionView.State

The states that tell users how to proceed when connecting to and switching between peripherals in a playground page.

