

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManager(\_:didDisconnectPeripheral:timestamp:isReconnecting:error:) 

Instance Method

# centralManager(\_:didDisconnectPeripheral:timestamp:isReconnecting:error:)

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func centralManager(
    _ central: CBCentralManager,
    didDisconnectPeripheral peripheral: CBPeripheral,
    timestamp: CFAbsoluteTime,
    isReconnecting: Bool,
    error: (any Error)?
)
```

