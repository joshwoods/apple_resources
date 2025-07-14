

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManagerDidUpdateState(\_:) 

Instance Method

# peripheralManagerDidUpdateState(\_:)

Tells the delegate the peripheral manager’s state updated.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func peripheralManagerDidUpdateState(_ peripheral: CBPeripheralManager)
```

**Required**

## Parameters 

`peripheral`  

The peripheral manager whose state has changed.

## Discussion

You implement this required method to ensure that Bluetooth low energy is available to use on the local peripheral device.

Issue commands to the peripheral manager only when the peripheral manager is in the powered-on state, as indicated by the CBPeripheralManagerState.poweredOn constant. A state with a value lower than CBPeripheralManagerState.poweredOn implies that advertising has stopped and that any connected centrals have been disconnected. If the state moves below CBPeripheralManagerState.poweredOff, advertising has stopped you must explicitly restart it. In addition, the powered off state clears the local database; in this case you must explicitly re-add all services. For a complete list and discussion of the possible values representing the state of the peripheral manager, see the CBPeripheralManagerState enumeration in CBPeripheralManager.

For more information, see Core Bluetooth Programming Guide.

## See Also

### Monitoring Changes to the Peripheral Manager’s State

func peripheralManager(CBPeripheralManager, willRestoreState: [String : Any])

Tells the delegate the system is about to restore the peripheral manager.

Peripheral Manager State Restoration Options

Keys used to specify options when restoring the state of a peripheral manager.

