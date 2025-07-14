

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManager(\_:connectionEventDidOccur:for:) 

Instance Method

# centralManager(\_:connectionEventDidOccur:for:)

Tells the delegate that a connection event occurred which matches the registered options.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
optional func centralManager(
    _ central: CBCentralManager,
    connectionEventDidOccur event: CBConnectionEvent,
    for peripheral: CBPeripheral
)
```

## Discussion

The manager calls this method when it observes a connection event that matches the options provided to registerForConnectionEvents(options:).

## See Also

### Monitoring Connections with Peripherals

func centralManager(CBCentralManager, didConnect: CBPeripheral)

Tells the delegate that the central manager connected to a peripheral.

func centralManager(CBCentralManager, didDisconnectPeripheral: CBPeripheral, error: (any Error)?)

Tells the delegate that the central manager disconnected from a peripheral.

func centralManager(CBCentralManager, didFailToConnect: CBPeripheral, error: (any Error)?)

Tells the delegate the central manager failed to create a connection with a peripheral.

