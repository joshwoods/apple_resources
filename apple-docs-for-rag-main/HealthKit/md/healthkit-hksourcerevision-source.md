

- HealthKit
- HKSourceRevision
-  source 

Instance Property

# source

The source for a sample.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var source: HKSource { get }
```

## Discussion

This property contains an HKSource object representing the app that saved the data into the HealthKit store. The source can also represent a hardware device that writes data directly to HealthKit (for example, an iPhone, Apple Watch, or Bluetooth LE heart rate monitor). Before iOS 9.0, the companion app for other peripherals also saved device information in the object’s source property.

## See Also

### Accessing Source and Version Information

var version: String?

A string that identifies a particular version of the source.

var operatingSystemVersion: OperatingSystemVersion

A string that identifies the operating system used to save a sample.

var productType: String?

A string that identifies the device used to save a sample.

