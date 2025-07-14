

- Core Media I/O
- CMIOExtensionDeviceProperties
-  transportType 

Instance Property

# transportType

The transport type of the device, such as USB or HDMI.

Mac Catalyst 15.4+macOS 12.3+Xcode 13.0+

``` source
@nonobjc
var transportType: Int? { get set }
```

## Discussion

The value is an IOKit framework transport type constant (`kIOAudioDeviceTransportType`).

The key for this property is deviceTransportType.

## See Also

### Configuring Device Properties

var model: String?

A device model string.

var linkedCoreAudioDeviceUID: String?

A universal identifier of the audio device linked to this device.

var suspended: Bool?

A Boolean value that indicates whether the device is in a suspended state.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets the value of a device property.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a device.

