

- Core Bluetooth
- CBPeripheral
-  services 

Instance Property

# services

A list of a peripheral’s discovered services.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var services: [CBService]? { get }
```

## Discussion

Returns an array of services (represented by CBService objects) that successful call to the discoverServices(_:) method discovered. If you haven’t yet called the discoverServices(_:) method to discover the services of the peripheral, or if there was an error in doing so, the value of this property is `nil`.

## See Also

### Discovering Services

func discoverServices([CBUUID]?)

Discovers the specified services of the peripheral.

func discoverIncludedServices([CBUUID]?, for: CBService)

Discovers the specified included services of a previously-discovered service.

