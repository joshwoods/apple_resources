

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManager(\_:didDisconnectPeripheral:error:) 

Instance Method

# centralManager(\_:didDisconnectPeripheral:error:)

Tells the delegate that the central manager disconnected from a peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func centralManager(
    _ central: CBCentralManager,
    didDisconnectPeripheral peripheral: CBPeripheral,
    error: (any Error)?
)
```

## Parameters 

`central`  

The central manager that provides this information.

`peripheral`  

The now-disconnected peripheral.

`error`  

The cause of the failure, or `nil` if no error occurred.

## Discussion

The manager invokes this method when disconnecting a peripheral previously connected with the connect(_:options:) method. The error parameter contains the reason for the disconnection, unless the disconnect resulted from a call to cancelPeripheralConnection(_:). After this method executes, the peripheral device’s CBPeripheralDelegate object receives no further method calls.

All services, characteristics, and characteristic descriptors a peripheral become invalidated after it disconnects.

## See Also

### Monitoring Connections with Peripherals

func centralManager(CBCentralManager, didConnect: CBPeripheral)

Tells the delegate that the central manager connected to a peripheral.

func centralManager(CBCentralManager, didFailToConnect: CBPeripheral, error: (any Error)?)

Tells the delegate the central manager failed to create a connection with a peripheral.

func centralManager(CBCentralManager, connectionEventDidOccur: CBConnectionEvent, for: CBPeripheral)

Tells the delegate that a connection event occurred which matches the registered options.

