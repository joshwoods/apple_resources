

- Core Bluetooth
- CBService
-  characteristics 

Instance Property

# characteristics

A list of characteristics discovered in this service.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var characteristics: [CBCharacteristic]? { get }
```

## Discussion

This array contains CBCharacteristic objects that represent a service’s characteristics. Characteristics provide further details about a peripheral’s service. For example, a heart rate service may contain one characteristic that describes the intended body location of the device’s heart rate sensor, while another characteristic transmits heart rate measurement data.

## See Also

### Accessing Service Data

var includedServices: [CBService]?

A list of included services discovered in this service.

