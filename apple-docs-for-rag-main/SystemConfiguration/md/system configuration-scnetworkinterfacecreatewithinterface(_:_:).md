

- System Configuration
-  SCNetworkInterfaceCreateWithInterface(\_:\_:) 

Function

# SCNetworkInterfaceCreateWithInterface(\_:\_:)

Creates a new network interface layered on top of the specified interface.

macOS 10.4+

``` source
func SCNetworkInterfaceCreateWithInterface(
    _ interface: SCNetworkInterface,
    _ interfaceType: CFString
) -> SCNetworkInterface?
```

## Parameters 

`interface`  

The network interface.

`interfaceType`  

The type of interface to layer on top of the network interface specified in `interface`.

## Return Value

A reference to the new network interface. You must release the returned value.

## Discussion

You can use this function to create a “PPP” interface on top of a “modem.”

## See Also

### Configuring Network Interfaces

func SCNetworkInterfaceCopyAll() -> CFArray

Returns all network-capable interfaces on the system.

func SCNetworkInterfaceCopyMTU(SCNetworkInterface, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?) -> Bool

Returns the current MTU setting and the range of allowable values for the specified network interface.

func SCNetworkInterfaceCopyMediaOptions(SCNetworkInterface, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>?, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>?, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>?, Bool) -> Bool

Returns information media options for the specified network interface.

func SCNetworkInterfaceCopyMediaSubTypeOptions(CFArray, CFString) -> CFArray?

Returns a list of available media options for the specified interface configuration options and subtype.

func SCNetworkInterfaceCopyMediaSubTypes(CFArray) -> CFArray?

Returns a list of available media subtypes for the specified interface configuration options.

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

