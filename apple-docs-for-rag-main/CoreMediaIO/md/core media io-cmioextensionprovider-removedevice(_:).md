

- Core Media I/O
- CMIOExtensionProvider
-  removeDevice(\_:) 

Instance Method

# removeDevice(\_:)

Removes a device from a provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
func removeDevice(_ device: CMIOExtensionDevice) throws
```

## Parameters 

`device`  

A device to remove from a provider.

## See Also

### Managing Devices

var devices: [CMIOExtensionDevice]

An array of connected devices.

func addDevice(CMIOExtensionDevice) throws

Adds a device to a provider.

