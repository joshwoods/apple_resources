

- DeviceDiscoveryUI
- DevicePickerSupportedAction
-  callAsFunction(\_:parameters:) 

Instance Method

# callAsFunction(\_:parameters:)

Returns a Boolean value that indicates whether the current device supports device discovery.

DeviceDiscoveryUISwiftUItvOS 16.0+

``` source
func callAsFunction(
    _ browseDescriptor: NWBrowser.Descriptor,
    parameters: (() -> NWParameters)? = nil
) -> Bool
```

## Parameters 

`browseDescriptor`  

A descriptor for your application service. To create an application service descriptor, call `NWBrowser.Descriptor.applicationService(name:options:)` and provide a name for the service.

`parameters`  

Parameters for your network connection. Use applicationService to create a default set of parameters that create an encrypted connection with the other devices. You can also add `a` NWProtocolFramer to provide an application-level messaging protocol.

