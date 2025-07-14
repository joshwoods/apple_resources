

- Core Media I/O
- CMIOExtensionDeviceProperties
-  linkedCoreAudioDeviceUID 

Instance Property

# linkedCoreAudioDeviceUID

A universal identifier of the audio device linked to this device.

Mac Catalyst 15.4+macOS 12.3+

``` source
var linkedCoreAudioDeviceUID: String? { get set }
```

## Discussion

The key for this property is deviceLinkedCoreAudioDeviceUID.

## See Also

### Configuring Device Properties

var model: String?

A device model string.

var transportType: Int?

The transport type of the device, such as USB or HDMI.

var suspended: Bool?

A Boolean value that indicates whether the device is in a suspended state.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets the value of a device property.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a device.

