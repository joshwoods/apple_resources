

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didOpen:error:) 

Instance Method

# peripheral(\_:didOpen:error:)

Delivers the result of an attempt to open an L2CAP channel.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didOpen channel: CBL2CAPChannel?,
    error: (any Error)?
)
```

## Discussion

This method delivers the result of a previous call to openL2CAPChannel(_:).

