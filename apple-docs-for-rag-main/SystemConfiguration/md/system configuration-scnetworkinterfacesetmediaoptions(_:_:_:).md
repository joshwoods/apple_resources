

- System Configuration
-  SCNetworkInterfaceSetMediaOptions(\_:\_:\_:) 

Function

# SCNetworkInterfaceSetMediaOptions(\_:\_:\_:)

Sets the requested media subtype and options for the specified network interface.

macOS 10.5+

``` source
func SCNetworkInterfaceSetMediaOptions(
    _ interface: SCNetworkInterface,
    _ subtype: CFString?,
    _ options: CFArray?
) -> Bool
```

## Parameters 

`interface`  

The network interface.

`subtype`  

The media subtype to set (for example, “autoselect” or “100baseTX”).

`options`  

The media options to set (for example, “half-duplex” or “full-duplex”). If `NULL`, the active options are not returned.

## Return Value

`TRUE` if the configuration was updated; `FALSE` if an error occurred.

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

