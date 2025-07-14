

- Core Media I/O
- CMIOExtensionProvider
-  devices 

Instance Property

# devices

An array of connected devices.

Mac Catalyst 15.4+macOS 12.3+

``` source
var devices: [CMIOExtensionDevice] { get }
```

## Discussion

This property isn’t key-value observable.

## See Also

### Managing Devices

func addDevice(CMIOExtensionDevice) throws

Adds a device to a provider.

func removeDevice(CMIOExtensionDevice) throws

Removes a device from a provider.

