

- Core Media I/O
- CMIOExtensionDeviceProperties
-  model 

Instance Property

# model

A device model string.

Mac Catalyst 15.4+macOS 12.3+

``` source
var model: String? { get set }
```

## Discussion

The key for this property is deviceModel.

## See Also

### Configuring Device Properties

var linkedCoreAudioDeviceUID: String?

A universal identifier of the audio device linked to this device.

var transportType: Int?

The transport type of the device, such as USB or HDMI.

var suspended: Bool?

A Boolean value that indicates whether the device is in a suspended state.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets the value of a device property.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a device.

