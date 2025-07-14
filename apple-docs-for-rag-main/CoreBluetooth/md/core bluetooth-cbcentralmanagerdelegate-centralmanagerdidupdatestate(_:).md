

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManagerDidUpdateState(\_:) 

Instance Method

# centralManagerDidUpdateState(\_:)

Tells the delegate the central manager’s state updated.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func centralManagerDidUpdateState(_ central: CBCentralManager)
```

**Required**

## Parameters 

`central`  

The central manager whose state has changed.

## Discussion

You implement this required method to ensure that the central device supports Bluetooth low energy and that it’s available to use. You should issue commands to the central manager only when the central manager’s state indicates it’s powered on. A state with a value lower than CBManagerState.poweredOn implies that scanning has stopped, which in turn disconnects any previously-connected peripherals. If the state moves below CBManagerState.poweredOff, all CBPeripheral objects obtained from this central manager become invalid; you must retrieve or discover these peripherals again. For a complete list of possible states, see CBManagerState.

## See Also

### Monitoring the Central Manager’s State

func centralManager(CBCentralManager, willRestoreState: [String : Any])

Tells the delegate the system is about to restore the central manager, as part of relaunching the app into the background.

