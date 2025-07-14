

- SensorKit
- SRDevice
-  productType 

Instance Property

# productType

A string that identifies the device used to save a sample.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var productType: String { get }
```

## Discussion

Note

Samples saved using older versions of SensorKit may have a `nil`-valued product type that indicates the product type is unknown.

## See Also

### Accessing Device Information

var model: String

The user-defined name of the device.

var name: String

The framework-defined name of the device.

var systemName: String

The device’s operating system.

var systemVersion: String

The device’s operating system version.

