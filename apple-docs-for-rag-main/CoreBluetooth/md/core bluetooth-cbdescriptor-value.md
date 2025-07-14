

- Core Bluetooth
- CBDescriptor
-  value 

Instance Property

# value

The value of the descriptor.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var value: Any? { get }
```

## Discussion

The documentation for CBUUID details the value types for the various descriptor types.

You can read the value of a descriptor by calling the readValue(for:) method of the CBPeripheral class. You can write the value of a descriptor by calling the writeValue(_:for:) method of the CBPeripheral class. You can’t, however, use the writeValue(_:for:) method to write the value of a client configuration descriptor (CBUUIDClientCharacteristicConfigurationString). Instead, you use the setNotifyValue(_:for:) method of the CBPeripheral class to configure client indications or notifications of a characteristic’s value on a server.

