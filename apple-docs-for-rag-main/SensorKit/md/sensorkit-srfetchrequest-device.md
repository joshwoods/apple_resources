

- SensorKit
- SRFetchRequest
-  device 

Instance Property

# device

The device to query for sample data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var device: SRDevice { get set }
```

## Discussion

If the app doesn’t define a value for this property, the framework queries the current device. To get a list of available devices, the app calls fetchDevices() on its sensor reader.

## See Also

### Selecting the Device

class SRDevice

A representation of a device that provides sample data.

