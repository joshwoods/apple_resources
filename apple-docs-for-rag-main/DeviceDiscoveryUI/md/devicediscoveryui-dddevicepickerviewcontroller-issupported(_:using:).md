

- DeviceDiscoveryUI
- DDDevicePickerViewController
-  isSupported(\_:using:) 

Type Method

# isSupported(\_:using:)

Returns a Boolean value that indicates whether the current device supports device discovery.

tvOS 16.0+

``` source
@MainActor @preconcurrency
static func isSupported(
    _ browseDescriptor: NWBrowser.Descriptor,
    using: NWParameters? = nil
) -> Bool
```

## Parameters 

`browseDescriptor`  

A descriptor for your application service. To create an application service descriptor, call `NWBrowser.Descriptor.applicationService(name:options:)` and provide a name for the service.

## See Also

### Creating device picker view controllers

convenience init?(browseDescriptor: NWBrowser.Descriptor, parameters: NWParameters?)

Creates a view controller that displays the other, available devices on your local network.

