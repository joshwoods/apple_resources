

- System Configuration
-  SCNetworkProtocolGetTypeID() 

Function

# SCNetworkProtocolGetTypeID()

Returns the type identifier of all `SCNetworkProtocol` instances.

macOS 10.4+

``` source
func SCNetworkProtocolGetTypeID() -> CFTypeID
```

## Return Value

The type identifier of all `SCNetworkProtocol` instances.

## See Also

### Configuring Network Protocols

func SCNetworkProtocolGetConfiguration(SCNetworkProtocol) -> CFDictionary?

Returns the configuration settings associated with the specified protocol.

func SCNetworkProtocolGetEnabled(SCNetworkProtocol) -> Bool

Returns a Boolean value indicating whether the specified protocol is enabled.

func SCNetworkProtocolGetProtocolType(SCNetworkProtocol) -> CFString?

Returns the type of the specified network protocol.

func SCNetworkProtocolSetConfiguration(SCNetworkProtocol, CFDictionary?) -> Bool

Stores the configuration settings for the specified network protocol.

func SCNetworkProtocolSetEnabled(SCNetworkProtocol, Bool) -> Bool

Enables or disables the specified protocol.

