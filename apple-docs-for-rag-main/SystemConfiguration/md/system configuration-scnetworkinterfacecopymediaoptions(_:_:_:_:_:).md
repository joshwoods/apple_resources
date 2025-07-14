

- System Configuration
-  SCNetworkInterfaceCopyMediaOptions(\_:\_:\_:\_:\_:) 

Function

# SCNetworkInterfaceCopyMediaOptions(\_:\_:\_:\_:\_:)

Returns information media options for the specified network interface.

macOS 10.5+

``` source
func SCNetworkInterfaceCopyMediaOptions(
    _ interface: SCNetworkInterface,
    _ current: UnsafeMutablePointer?>?,
    _ active: UnsafeMutablePointer?>?,
    _ available: UnsafeMutablePointer?>?,
    _ filter: Bool
) -> Bool
```

## Parameters 

`interface`  

The network interface.

`current`  

On output, a dictionary representing the currently requested media options (subtype, options). If `NULL`, the current options are not returned.

`active`  

On output, a dictionary representing the active media options (subtype, options). If `NULL`, the active options are not returned.

`available`  

On output, an array representing the possible media options (subtype, options). If `NULL`, the current options are not returned.

`filter`  

A Boolean value indicating whether the available options should be filtered to exclude those options which would not normally be requested by a user/admin (for example, `hw-loopback`).

## Return Value

`TRUE` if requested information has been returned.

## See Also

### Configuring Network Interfaces

func SCNetworkInterfaceCopyAll() -> CFArray

Returns all network-capable interfaces on the system.

func SCNetworkInterfaceCopyMTU(SCNetworkInterface, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?) -> Bool

Returns the current MTU setting and the range of allowable values for the specified network interface.

func SCNetworkInterfaceCopyMediaSubTypeOptions(CFArray, CFString) -> CFArray?

Returns a list of available media options for the specified interface configuration options and subtype.

func SCNetworkInterfaceCopyMediaSubTypes(CFArray) -> CFArray?

Returns a list of available media subtypes for the specified interface configuration options.

func SCNetworkInterfaceCreateWithInterface(SCNetworkInterface, CFString) -> SCNetworkInterface?

Creates a new network interface layered on top of the specified interface.

func SCNetworkInterfaceForceConfigurationRefresh(SCNetworkInterface) -> Bool

Sends a notification to interested network configuration agents to immediately retry their configuration.

func SCNetworkInterfaceGetBSDName(SCNetworkInterface) -> CFString?

Returns the BSD interface or device name for the specified interface.

func SCNetworkInterfaceGetConfiguration(SCNetworkInterface) -> CFDictionary?

Returns the configuration settings associated with the specified interface.

func SCNetworkInterfaceGetExtendedConfiguration(SCNetworkInterface, CFString) -> CFDictionary?

Returns the extended configuration settings associated with the specified interface.

func SCNetworkInterfaceGetHardwareAddressString(SCNetworkInterface) -> CFString?

Returns a displayable link layer address for the specified interface.

func SCNetworkInterfaceGetInterface(SCNetworkInterface) -> SCNetworkInterface?

Returns the underlying interface, for layered network interfaces.

func SCNetworkInterfaceGetInterfaceType(SCNetworkInterface) -> CFString?

Returns the network interface type of the specified interface.

func SCNetworkInterfaceGetLocalizedDisplayName(SCNetworkInterface) -> CFString?

Returns the localized display name, such as “Ethernet” or “FireWire”, for the specified interface.

func SCNetworkInterfaceGetSupportedInterfaceTypes(SCNetworkInterface) -> CFArray?

Identifies all of the network interface types, such as PPP, that can be layered on top of the specified interface.

func SCNetworkInterfaceGetSupportedProtocolTypes(SCNetworkInterface) -> CFArray?

Identifies all of the network protocol types, such as IPv4 and IPv6, that can be layered on top of the specified interface.

