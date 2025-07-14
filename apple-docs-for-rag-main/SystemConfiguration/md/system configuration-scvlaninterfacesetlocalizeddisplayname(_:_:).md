

- System Configuration
-  SCVLANInterfaceSetLocalizedDisplayName(\_:\_:) 

Function

# SCVLANInterfaceSetLocalizedDisplayName(\_:\_:)

Sets the localized display name for the specified virtual LAN (VLAN) interface.

macOS 10.5+

``` source
func SCVLANInterfaceSetLocalizedDisplayName(
    _ vlan: SCVLANInterface,
    _ newName: CFString
) -> Bool
```

## Parameters 

`vlan`  

The VLAN interface.

`newName`  

The new display name.

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

func SCVLANInterfaceSetOptions(SCVLANInterface, CFDictionary) -> Bool

Sets the specified configuration settings for the specified virtual LAN (VLAN) interface.

func SCVLANInterfaceSetPhysicalInterfaceAndTag(SCVLANInterface, SCNetworkInterface, CFNumber) -> Bool

Updates the specified virtual LAN (VLAN) interface with the specified information.

