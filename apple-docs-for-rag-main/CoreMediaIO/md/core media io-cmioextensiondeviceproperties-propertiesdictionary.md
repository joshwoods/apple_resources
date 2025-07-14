

- Core Media I/O
- CMIOExtensionDeviceProperties
-  propertiesDictionary 

Instance Property

# propertiesDictionary

A dictionary of properties for a device.

Mac Catalyst 15.4+macOS 12.3+

``` source
var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState] { get set }
```

## See Also

### Configuring Device Properties

var model: String?

A device model string.

var linkedCoreAudioDeviceUID: String?

A universal identifier of the audio device linked to this device.

var transportType: Int?

The transport type of the device, such as USB or HDMI.

var suspended: Bool?

A Boolean value that indicates whether the device is in a suspended state.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets the value of a device property.

