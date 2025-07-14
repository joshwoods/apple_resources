

- System Configuration
-  SCVLANInterfaceSetPhysicalInterfaceAndTag(\_:\_:\_:) 

Function

# SCVLANInterfaceSetPhysicalInterfaceAndTag(\_:\_:\_:)

Updates the specified virtual LAN (VLAN) interface with the specified information.

macOS 10.5+

``` source
func SCVLANInterfaceSetPhysicalInterfaceAndTag(
    _ vlan: SCVLANInterface,
    _ physical: SCNetworkInterface,
    _ tag: CFNumber
) -> Bool
```

## Parameters 

`vlan`  

The VLAN interface to update.

`physical`  

The physical interface to associate with the VLAN interface.

`tag`  

The tag to associate with the VLAN interface. This value must be between 1 and 4094.

## Return Value

`TRUE` if the configuration was stored; `FALSE` if an error occurred.

## See Also

### Configuring VLAN Interfaces

func SCVLANInterfaceCopyAll(SCPreferences) -> CFArray

Returns all virtual LAN (VLAN) interfaces on the system.

func SCVLANInterfaceCopyAvailablePhysicalInterfaces() -> CFArray

Returns the network capable devices on the system that can be associated with a virtual LAN (VLAN) interface.

func SCVLANInterfaceCreate(SCPreferences, SCNetworkInterface, CFNumber) -> SCVLANInterface?

Creates a new virtual LAN (VLAN) interface.

func SCVLANInterfaceGetOptions(SCVLANInterface) -> CFDictionary?

Returns the configuration settings associated with the virtual LAN (VLAN) interface.

func SCVLANInterfaceGetPhysicalInterface(SCVLANInterface) -> SCNetworkInterface?

Returns the physical interface for the specified virtual LAN (VLAN) interface.

func SCVLANInterfaceGetTag(SCVLANInterface) -> CFNumber?

Returns the tag for the specified virtual LAN (VLAN) interface.

func SCVLANInterfaceRemove(SCVLANInterface) -> Bool

Removes the virtual LAN (VLAN) interface from the configuration.

func SCVLANInterfaceSetLocalizedDisplayName(SCVLANInterface, CFString) -> Bool

Sets the localized display name for the specified virtual LAN (VLAN) interface.

func SCVLANInterfaceSetOptions(SCVLANInterface, CFDictionary) -> Bool

Sets the specified configuration settings for the specified virtual LAN (VLAN) interface.

