

- DeviceDiscoveryUI
- DevicePicker
-  init(\_:onSelect:label:fallback:parameters:) 

Initializer

# init(\_:onSelect:label:fallback:parameters:)

Creates a view that displays the other, available devices on your local network.

DeviceDiscoveryUISwiftUItvOS 16.0+

``` source
@MainActor @preconcurrency
init(
    _ browseDescriptor: NWBrowser.Descriptor,
    onSelect: @escaping (NWEndpoint) -> Void,
    @ViewBuilder label: () -> Label,
    @ViewBuilder fallback: () -> Fallback,
    parameters: (() -> NWParameters)? = nil
)
```

## Parameters 

`browseDescriptor`  

A descriptor for your application service. To create an application service descriptor, call `NWBrowser.Descriptor.applicationService(name:options:)` and provide a name for the service.

`onSelect`  

A closure that the system calls when the user selects a device in the picker view, or cancels the view.

`label`  

A label displayed by the network device picker.

`fallback`  

A view that the system displays if the current device doesn’t support device discovery.

`parameters`  

Parameters for your network connection. Use applicationService to create a default set of parameters that create an encrypted connection with the other devices. You can also add `a` NWProtocolFramer to provide an application-level messaging protocol.

