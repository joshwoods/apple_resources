

- System Configuration
-  SCVLANInterfaceGetPhysicalInterface(\_:) 

Function

# SCVLANInterfaceGetPhysicalInterface(\_:)

Returns the physical interface for the specified virtual LAN (VLAN) interface.

macOS 10.5+

``` source
func SCVLANInterfaceGetPhysicalInterface(_ vlan: SCVLANInterface) -> SCNetworkInterface?
```

## Parameters 

`vlan`  

The VLAN interface.

## Return Value

The list of interfaces.

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

func SCVLANInterfaceGetTag(SCVLANInterface) -> CFNumber?

Returns the tag for the specified virtual LAN (VLAN) interface.

func SCVLANInterfaceRemove(SCVLANInterface) -> Bool

Removes the virtual LAN (VLAN) interface from the configuration.

func SCVLANInterfaceSetLocalizedDisplayName(SCVLANInterface, CFString) -> Bool

Sets the localized display name for the specified virtual LAN (VLAN) interface.

func SCVLANInterfaceSetOptions(SCVLANInterface, CFDictionary) -> Bool

Sets the specified configuration settings for the specified virtual LAN (VLAN) interface.

func SCVLANInterfaceSetPhysicalInterfaceAndTag(SCVLANInterface, SCNetworkInterface, CFNumber) -> Bool

Updates the specified virtual LAN (VLAN) interface with the specified information.

