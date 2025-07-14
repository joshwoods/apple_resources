

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  setItem(\_:forPeripheral:) 

Instance Method

# setItem(\_:forPeripheral:)

Sets all of the information about the specified peripheral at once.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func setItem(
    _ item: PlaygroundBluetoothConnectionView.Item,
    forPeripheral peripheral: CBPeripheral
)
```

## Parameters 

`item`  

A PlaygroundBluetoothConnectionView.Item that holds information about the specified peripheral.

`peripheral`  

The peripheral corresponding to the `PlaygroundBluetoothConnectionView.Item` being displayed.

## See Also

### Displaying Peripherals

struct PlaygroundBluetoothConnectionView.Item

A value that holds information about a peripheral displayed in a connection view.

