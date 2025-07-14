

- Core Bluetooth
- CBMutableService
-  characteristics 

Instance Property

# characteristics

A list of characteristics of a service.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var characteristics: [CBCharacteristic]? { get set }
```

## Discussion

An array containing CBCharacteristic objects that represent a service’s characteristics. Characteristics provide further details about a peripheral’s service. For example, a heart rate service may contain one characteristic that describes the intended body location of the device’s heart rate sensor, while another characteristic transmits heart rate measurement data.

## See Also

### Managing a Mutable Service

var includedServices: [CBService]?

A list of included services.

