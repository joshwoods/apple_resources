

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
-  connectToLastConnectedPeripheral(timeout:callback:) 

Instance Method

# connectToLastConnectedPeripheral(timeout:callback:)

Attempts to reconnect the central manager to the most recently connected peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connectToLastConnectedPeripheral(
    timeout: TimeInterval = 7.0,
    callback: ((CBPeripheral?, Error?) -> Void)? = nil
) -> Bool
```

## Parameters 

`timeout`  

The amount of time, in seconds, before the connection attempt is aborted. If the timeout value is `nil`, the attempt won’t time out. To cancel a connection attempt, call the disconnect(from:) method.

`callback`  

A function that’s called when the connection attempt succeeds or fails.

## Return Value

A Boolean value indicating whether the currently active playground book has previously connected to a peripheral. If `true`, the central manager attempts to reconnect to it.

## See Also

### Connecting Peripherals

func connect(to: CBPeripheral, timeout: TimeInterval?, callback: ((CBPeripheral, Error?) -> Void)?)

Attempts to connect the central manager to the specified peripheral.

func connect(toPeripheralWithUUID: UUID, timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?)

Attempts to connect the central manager to a peripheral with the specified unique identifier.

enum PlaygroundBluetoothCentralManager.ConnectionError

The errors you may encounter when connecting a peripheral to the central manager for the current playground page.

