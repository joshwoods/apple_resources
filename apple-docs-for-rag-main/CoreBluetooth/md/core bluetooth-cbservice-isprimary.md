

- Core Bluetooth
- CBService
-  isPrimary 

Instance Property

# isPrimary

A Boolean value that indicates whether the type of service is primary or secondary.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isPrimary: Bool { get }
```

## Discussion

A peripheral’s service is either primary or secondary. A primary service describes the primary function of a device. A secondary service describes a service that’s relevant only in the context of another service that references it. For example, the primary service of a heart rate monitor may be to expose heart rate data from the monitor’s heart rate sensor. In this example, a secondary service may be to expose the sensor’s battery data.

If the value of this property is true, the type of service is primary. If the value of this property is false, the type of service is secondary.

## See Also

### Identifying a Service

var peripheral: CBPeripheral?

The peripheral to which this service belongs.

