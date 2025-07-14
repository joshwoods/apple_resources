

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
-  connect(to:timeout:callback:) 

Instance Method

# connect(to:timeout:callback:)

Attempts to connect the central manager to the specified peripheral.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
func connect(
    to peripheral: CBPeripheral,
    timeout: TimeInterval? = nil,
    callback: ((CBPeripheral, Error?) -> Void)? = nil
)
```

## Parameters 

`peripheral`  

The peripheral to attempt to connect to.

`timeout`  

The amount of time, in seconds, before the connection attempt is aborted. If the timeout value is `nil`, the attempt won’t time out. To cancel a connection attempt, call the disconnect(from:) method.

`callback`  

A function that’s called when the connection attempt succeeds or fails.

## See Also

### Connecting Peripherals

func connect(toPeripheralWithUUID: UUID, timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?)

Attempts to connect the central manager to a peripheral with the specified unique identifier.

func connectToLastConnectedPeripheral(timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?) -> Bool

Attempts to reconnect the central manager to the most recently connected peripheral.

enum PlaygroundBluetoothCentralManager.ConnectionError

The errors you may encounter when connecting a peripheral to the central manager for the current playground page.

