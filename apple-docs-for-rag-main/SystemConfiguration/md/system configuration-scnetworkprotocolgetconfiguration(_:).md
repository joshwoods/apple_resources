

- System Configuration
-  SCNetworkProtocolGetConfiguration(\_:) 

Function

# SCNetworkProtocolGetConfiguration(\_:)

Returns the configuration settings associated with the specified protocol.

macOS 10.4+

``` source
func SCNetworkProtocolGetConfiguration(_ protocol: SCNetworkProtocol) -> CFDictionary?
```

## Parameters 

`protocol`  

The network protocol.

## Return Value

The configuration settings associated with the protocol, or `NULL` if no configuration settings are associated with the protocol or an error occurred.

## See Also

### Configuring Network Protocols

func SCNetworkProtocolGetEnabled(SCNetworkProtocol) -> Bool

Returns a Boolean value indicating whether the specified protocol is enabled.

func SCNetworkProtocolGetProtocolType(SCNetworkProtocol) -> CFString?

Returns the type of the specified network protocol.

func SCNetworkProtocolGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkProtocol` instances.

func SCNetworkProtocolSetConfiguration(SCNetworkProtocol, CFDictionary?) -> Bool

Stores the configuration settings for the specified network protocol.

func SCNetworkProtocolSetEnabled(SCNetworkProtocol, Bool) -> Bool

Enables or disables the specified protocol.

