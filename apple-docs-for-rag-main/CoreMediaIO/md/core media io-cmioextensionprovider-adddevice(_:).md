

- Core Media I/O
- CMIOExtensionProvider
-  addDevice(\_:) 

Instance Method

# addDevice(\_:)

Adds a device to a provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
func addDevice(_ device: CMIOExtensionDevice) throws
```

## Parameters 

`device`  

A device to add to a provider.

## See Also

### Managing Devices

var devices: [CMIOExtensionDevice]

An array of connected devices.

func removeDevice(CMIOExtensionDevice) throws

Removes a device from a provider.

