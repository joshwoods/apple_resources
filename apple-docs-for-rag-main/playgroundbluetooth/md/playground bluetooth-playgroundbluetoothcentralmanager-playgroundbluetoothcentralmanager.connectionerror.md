

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
-  PlaygroundBluetoothCentralManager.ConnectionError 

Enumeration

# PlaygroundBluetoothCentralManager.ConnectionError

The errors you may encounter when connecting a peripheral to the central manager for the current playground page.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
enum PlaygroundBluetoothCentralManager.ConnectionError
```

## Topics

### Handling Errors

case connectionFailed

The error that occurs when a peripheral fails to connect to the central manager.

case connectionLost

The error that occurs when a peripheral connection to the central manager fails.

case excessiveConnections

The error that occurs when a peripheral rejects a connection to the central manager because there are too many others.

case invalidState

The error that occurs when the central manager is in a state that can’t make connections.

case timeoutExpired

The error that occurs when a peripheral fails to connect to the central manager before the timeout period expires.

### Displaying Errors

var localizedDescription: String

A string containing the localized description of the error.

### Comparing Errors

static func != (PlaygroundBluetoothCentralManager.ConnectionError, PlaygroundBluetoothCentralManager.ConnectionError) -> Bool

Returns `true` when the two connection errors being compared aren't the same.

## Relationships

### Conforms To

- Error

## See Also

### Connecting Peripherals

func connect(to: CBPeripheral, timeout: TimeInterval?, callback: ((CBPeripheral, Error?) -> Void)?)

Attempts to connect the central manager to the specified peripheral.

func connect(toPeripheralWithUUID: UUID, timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?)

Attempts to connect the central manager to a peripheral with the specified unique identifier.

func connectToLastConnectedPeripheral(timeout: TimeInterval, callback: ((CBPeripheral?, Error?) -> Void)?) -> Bool

Attempts to reconnect the central manager to the most recently connected peripheral.

