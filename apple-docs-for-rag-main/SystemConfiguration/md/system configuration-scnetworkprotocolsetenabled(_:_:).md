

- System Configuration
-  SCNetworkProtocolSetEnabled(\_:\_:) 

Function

# SCNetworkProtocolSetEnabled(\_:\_:)

Enables or disables the specified protocol.

macOS 10.4+

``` source
func SCNetworkProtocolSetEnabled(
    _ protocol: SCNetworkProtocol,
    _ enabled: Bool
) -> Bool
```

## Parameters 

`protocol`  

The network protocol to enable or disable.

`enabled`  

`TRUE` if the protocol should be enabled.

## Return Value

`TRUE` if the enabled status was saved; `FALSE` if an error occurred.

## See Also

### Configuring Network Protocols

func SCNetworkProtocolGetConfiguration(SCNetworkProtocol) -> CFDictionary?

Returns the configuration settings associated with the specified protocol.

func SCNetworkProtocolGetEnabled(SCNetworkProtocol) -> Bool

Returns a Boolean value indicating whether the specified protocol is enabled.

func SCNetworkProtocolGetProtocolType(SCNetworkProtocol) -> CFString?

Returns the type of the specified network protocol.

func SCNetworkProtocolGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkProtocol` instances.

func SCNetworkProtocolSetConfiguration(SCNetworkProtocol, CFDictionary?) -> Bool

Stores the configuration settings for the specified network protocol.

