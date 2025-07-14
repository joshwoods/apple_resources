

- Core Media I/O
- CMIOExtensionDeviceProperties
-  setPropertyState(\_:forProperty:) 

Instance Method

# setPropertyState(\_:forProperty:)

Sets the value of a device property.

Mac Catalyst 15.4+macOS 12.3+

``` source
func setPropertyState(
    _ propertyState: CMIOExtensionPropertyState?,
    forProperty property: CMIOExtensionProperty
)
```

## Parameters 

`propertyState`  

The updated property state.

`property`  

The property to update.

## Discussion

Setting a `nil` property state value doesn’t remove the property.

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

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a device.

