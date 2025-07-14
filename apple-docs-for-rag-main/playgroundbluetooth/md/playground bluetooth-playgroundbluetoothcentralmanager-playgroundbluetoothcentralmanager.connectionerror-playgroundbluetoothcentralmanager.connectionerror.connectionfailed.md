

- Playground Bluetooth
- PlaygroundBluetoothCentralManager
- PlaygroundBluetoothCentralManager.ConnectionError
-  PlaygroundBluetoothCentralManager.ConnectionError.connectionFailed 

Enumeration Case

# PlaygroundBluetoothCentralManager.ConnectionError.connectionFailed

The error that occurs when a peripheral fails to connect to the central manager.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
case connectionFailed
```

## See Also

### Handling Errors

case connectionLost

The error that occurs when a peripheral connection to the central manager fails.

case excessiveConnections

The error that occurs when a peripheral rejects a connection to the central manager because there are too many others.

case invalidState

The error that occurs when the central manager is in a state that can’t make connections.

case timeoutExpired

The error that occurs when a peripheral fails to connect to the central manager before the timeout period expires.

