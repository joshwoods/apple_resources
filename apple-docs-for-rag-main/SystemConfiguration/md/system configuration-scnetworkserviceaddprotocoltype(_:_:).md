

- System Configuration
-  SCNetworkServiceAddProtocolType(\_:\_:) 

Function

# SCNetworkServiceAddProtocolType(\_:\_:)

Adds the network protocol of the specified type to the specified service.

macOS 10.4+

``` source
func SCNetworkServiceAddProtocolType(
    _ service: SCNetworkService,
    _ protocolType: CFString
) -> Bool
```

## Parameters 

`service`  

The network service.

`protocolType`  

The type of network protocol to add to the service.

## Return Value

`TRUE` if the protocol was added to the service; `FALSE` if the protocol was already present or an error occurred.

## Discussion

The protocol configuration is set to default values that are appropriate for the interface associated with the service.

## See Also

### Configuring Network Services

func SCNetworkServiceCopy(SCPreferences, CFString) -> SCNetworkService?

Returns the network service with the specified identifier.

func SCNetworkServiceCopyAll(SCPreferences) -> CFArray?

Returns all available network services for the specified preferences.

func SCNetworkServiceCopyProtocol(SCNetworkService, CFString) -> SCNetworkProtocol?

Returns the network protocol of the specified type for the specified service.

func SCNetworkServiceCopyProtocols(SCNetworkService) -> CFArray?

Returns all network protocols associated with the specified service.

func SCNetworkServiceCreate(SCPreferences, SCNetworkInterface) -> SCNetworkService?

Creates a new network service for the specified interface in the configuration.

func SCNetworkServiceEstablishDefaultConfiguration(SCNetworkService) -> Bool

Establishes the default configuration for the specified network service.

func SCNetworkServiceGetEnabled(SCNetworkService) -> Bool

Returns a Boolean value indicating whether the specified service is enabled.

func SCNetworkServiceGetInterface(SCNetworkService) -> SCNetworkInterface?

Returns the network interface associated with the specified service.

func SCNetworkServiceGetName(SCNetworkService) -> CFString?

Returns the user-specified name associated with the specified service.

func SCNetworkServiceGetServiceID(SCNetworkService) -> CFString?

Returns the identifier for the specified service.

func SCNetworkServiceGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkService` instances.

func SCNetworkServiceRemove(SCNetworkService) -> Bool

Removes the specified network service from the configuration.

func SCNetworkServiceRemoveProtocolType(SCNetworkService, CFString) -> Bool

Removes the network protocol of the specified type from the specified service.

func SCNetworkServiceSetEnabled(SCNetworkService, Bool) -> Bool

Enables or disables the specified service.

func SCNetworkServiceSetName(SCNetworkService, CFString?) -> Bool

Stores the user-specified name for the specified service.

