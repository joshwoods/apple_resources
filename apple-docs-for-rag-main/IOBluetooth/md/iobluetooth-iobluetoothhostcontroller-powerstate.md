

- IOBluetooth
- IOBluetoothHostController
-  powerState 

Instance Property

# powerState

Gets the controller power state

macOS

``` source
var powerState: BluetoothHCIPowerState { get }
```

## Return Value

The current controller’s power state. This will be 1 for on, or 0 for off. Only Apple Bluetooth adapters support power off

