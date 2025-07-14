

- Playground Bluetooth
- PlaygroundBluetoothConnectionViewDelegate
-  connectionView(\_:firmwareUpdateInstructionsFor:) 

Instance Method

# connectionView(\_:firmwareUpdateInstructionsFor:)

Tells the delegate that a peripheral has a firmware update available.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connectionView(
    _ connectionView: PlaygroundBluetoothConnectionView,
    firmwareUpdateInstructionsFor peripheral: CBPeripheral
) -> String
```

**Required**

## Parameters 

`connectionView`  

The central manager that failed to make the new connection.

`peripheral`  

The peripheral that the central manager couldn’t connect to.

## Return Value

A localized string that contains firmware update instructions.

