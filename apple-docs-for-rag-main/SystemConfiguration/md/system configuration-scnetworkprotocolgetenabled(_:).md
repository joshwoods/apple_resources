

- System Configuration
-  SCNetworkProtocolGetEnabled(\_:) 

Function

# SCNetworkProtocolGetEnabled(\_:)

Returns a Boolean value indicating whether the specified protocol is enabled.

macOS 10.4+

``` source
func SCNetworkProtocolGetEnabled(_ protocol: SCNetworkProtocol) -> Bool
```

## Parameters 

`protocol`  

The network protocol.

## Return Value

`TRUE` if the protocol is enabled; otherwise, `FALSE`.

## See Also

### Configuring Network Protocols

func SCNetworkProtocolGetConfiguration(SCNetworkProtocol) -> CFDictionary?

Returns the configuration settings associated with the specified protocol.

func SCNetworkProtocolGetProtocolType(SCNetworkProtocol) -> CFString?

Returns the type of the specified network protocol.

func SCNetworkProtocolGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkProtocol` instances.

func SCNetworkProtocolSetConfiguration(SCNetworkProtocol, CFDictionary?) -> Bool

Stores the configuration settings for the specified network protocol.

func SCNetworkProtocolSetEnabled(SCNetworkProtocol, Bool) -> Bool

Enables or disables the specified protocol.

