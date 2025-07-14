

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManager(\_:didConnect:) 

Instance Method

# centralManager(\_:didConnect:)

Tells the delegate that the central manager connected to a peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func centralManager(
    _ central: CBCentralManager,
    didConnect peripheral: CBPeripheral
)
```

## Parameters 

`central`  

The central manager that provides this information.

`peripheral`  

The now-connected peripheral.

## Discussion

The manager invokes this method when a call to connect(_:options:) succeeds. You typically implement this method to set the peripheral’s delegate and discover its services.

For more information, see Core Bluetooth Programming Guide.

## See Also

### Monitoring Connections with Peripherals

func centralManager(CBCentralManager, didDisconnectPeripheral: CBPeripheral, error: (any Error)?)

Tells the delegate that the central manager disconnected from a peripheral.

func centralManager(CBCentralManager, didFailToConnect: CBPeripheral, error: (any Error)?)

Tells the delegate the central manager failed to create a connection with a peripheral.

func centralManager(CBCentralManager, connectionEventDidOccur: CBConnectionEvent, for: CBPeripheral)

Tells the delegate that a connection event occurred which matches the registered options.

