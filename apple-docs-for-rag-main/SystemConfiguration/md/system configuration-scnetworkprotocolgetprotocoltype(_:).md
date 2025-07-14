

- System Configuration
-  SCNetworkProtocolGetProtocolType(\_:) 

Function

# SCNetworkProtocolGetProtocolType(\_:)

Returns the type of the specified network protocol.

macOS 10.4+

``` source
func SCNetworkProtocolGetProtocolType(_ protocol: SCNetworkProtocol) -> CFString?
```

## Parameters 

`protocol`  

The network protocol.

## Return Value

The protocol type.

## See Also

### Configuring Network Protocols

func SCNetworkProtocolGetConfiguration(SCNetworkProtocol) -> CFDictionary?

Returns the configuration settings associated with the specified protocol.

func SCNetworkProtocolGetEnabled(SCNetworkProtocol) -> Bool

Returns a Boolean value indicating whether the specified protocol is enabled.

func SCNetworkProtocolGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkProtocol` instances.

func SCNetworkProtocolSetConfiguration(SCNetworkProtocol, CFDictionary?) -> Bool

Stores the configuration settings for the specified network protocol.

func SCNetworkProtocolSetEnabled(SCNetworkProtocol, Bool) -> Bool

Enables or disables the specified protocol.

