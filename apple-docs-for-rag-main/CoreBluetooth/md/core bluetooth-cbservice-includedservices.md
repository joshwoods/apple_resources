

- Core Bluetooth
- CBService
-  includedServices 

Instance Property

# includedServices

A list of included services discovered in this service.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var includedServices: [CBService]? { get }
```

## Discussion

This array contains CBService objects that represent the included services of a service. A service of a peripheral may contain a reference to other services that are available on the peripheral. These other services are the included services of the service. You discover included services using the discoverIncludedServices(_:for:) method of the CBPeripheral class.

## See Also

### Accessing Service Data

var characteristics: [CBCharacteristic]?

A list of characteristics discovered in this service.

