

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
-  connect(toPeripheralWithUUID:timeout:callback:) 

Instance Method

# connect(toPeripheralWithUUID:timeout:callback:)

Attempts to connect the central manager to a peripheral with the specified unique identifier.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connect(
    toPeripheralWithUUID uuid: UUID,
    timeout: TimeInterval = 7,
    callback: ((CBPeripheral?, Error?) -> Void)? = nil
)
```

## Parameters 

`uuid`  

The unique identifier of the peripheral to attempt to connect to.

`timeout`  

The amount of time, in seconds, before the connection attempt is aborted. If the timeout value is `nil`, the attempt won’t time out. To cancel a connection attempt, call the disconnect(from:) method.

`callback`  

A function that’s called when the connection attempt succeeds or fails.

## See Also

### Connecting Peripherals

func connect(to: CBPeripheral, timeout: TimeInterval?, callback: ((CBPeripheral, Error?) -> Void)?)

Attempts to connect the central manager to the specified peripheral.

func connectToLastConnectedPeripheral(timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?) -> Bool

Attempts to reconnect the central manager to the most recently connected peripheral.

enum PlaygroundBluetoothCentralManager.ConnectionError

The errors you may encounter when connecting a peripheral to the central manager for the current playground page.

