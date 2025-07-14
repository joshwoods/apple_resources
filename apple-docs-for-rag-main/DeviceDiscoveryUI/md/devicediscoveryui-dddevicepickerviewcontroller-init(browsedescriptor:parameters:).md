

- DeviceDiscoveryUI
- DDDevicePickerViewController
-  init(browseDescriptor:parameters:) 

Initializer

# init(browseDescriptor:parameters:)

Creates a view controller that displays the other, available devices on your local network.

tvOS 16.0+

``` source
@MainActor @preconcurrency
convenience init?(
    browseDescriptor: NWBrowser.Descriptor,
    parameters: NWParameters? = nil
)
```

## Parameters 

`browseDescriptor`  

A descriptor for your application service. To create an application service descriptor, call `NWBrowser.Descriptor.applicationService(name:options:)` and provide a name for the service.

`parameters`  

Parameters for your network connection. Use applicationService to create a default set of parameters that create an encrypted connection with the other devices. You can also add `a` NWProtocolFramer to provide an application-level messaging protocol.

## See Also

### Creating device picker view controllers

static func isSupported(NWBrowser.Descriptor, using: NWParameters?) -> Bool

Returns a Boolean value that indicates whether the current device supports device discovery.

