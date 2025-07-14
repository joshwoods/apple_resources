

- System Configuration
-  SCNetworkProtocolSetConfiguration(\_:\_:) 

Function

# SCNetworkProtocolSetConfiguration(\_:\_:)

Stores the configuration settings for the specified network protocol.

macOS 10.4+

``` source
func SCNetworkProtocolSetConfiguration(
    _ protocol: SCNetworkProtocol,
    _ config: CFDictionary?
) -> Bool
```

## Parameters 

`protocol`  

The network protocol.

`config`  

The configuration settings to store.

## Return Value

`TRUE` if the configuration was stored; `FALSE` if an error occurred.

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

func SCNetworkProtocolSetEnabled(SCNetworkProtocol, Bool) -> Bool

Enables or disables the specified protocol.

