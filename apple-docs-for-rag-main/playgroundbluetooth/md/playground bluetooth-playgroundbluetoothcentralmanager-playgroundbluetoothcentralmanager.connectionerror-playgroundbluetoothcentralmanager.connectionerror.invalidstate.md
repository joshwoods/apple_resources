

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
- PlaygroundBluetoothCentralManager.ConnectionError
-  PlaygroundBluetoothCentralManager.ConnectionError.invalidState 

Enumeration Case

# PlaygroundBluetoothCentralManager.ConnectionError.invalidState

The error that occurs when the central manager is in a state that can’t make connections.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case invalidState
```

## Discussion

For example, the central manager is in an invalid state for connections when it’s powered off.

## See Also

### Handling Errors

case connectionFailed

The error that occurs when a peripheral fails to connect to the central manager.

case connectionLost

The error that occurs when a peripheral connection to the central manager fails.

case excessiveConnections

The error that occurs when a peripheral rejects a connection to the central manager because there are too many others.

case timeoutExpired

The error that occurs when a peripheral fails to connect to the central manager before the timeout period expires.

