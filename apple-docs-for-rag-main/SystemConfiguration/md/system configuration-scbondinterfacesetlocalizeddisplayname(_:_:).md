

- System Configuration
-  SCBondInterfaceSetLocalizedDisplayName(\_:\_:) 

Function

# SCBondInterfaceSetLocalizedDisplayName(\_:\_:)

Sets the localized display name for the specified Ethernet bond interface.

macOS 10.5+

``` source
func SCBondInterfaceSetLocalizedDisplayName(
    _ bond: SCBondInterface,
    _ newName: CFString
) -> Bool
```

## Parameters 

`bond`  

The Ethernet bond interface.

`newName`  

The new display name.

## Return Value

`TRUE` if the configuration was stored; `FALSE` if an error occurred.

## See Also

### Configuring Ethernet Bond Interfaces

func SCBondInterfaceCopyAll(SCPreferences) -> CFArray

Returns all Ethernet bond interfaces on the system.

func SCBondInterfaceCopyAvailableMemberInterfaces(SCPreferences) -> CFArray

Returns all network capable devices on the system that can be added to an Ethernet bond interface.

func SCBondInterfaceCopyStatus(SCBondInterface) -> SCBondStatus?

Returns the status of the specified Ethernet bond interface.

func SCBondInterfaceCreate(SCPreferences) -> SCBondInterface?

Creates a new Ethernet bond interface.

func SCBondInterfaceGetMemberInterfaces(SCBondInterface) -> CFArray?

Returns the member interfaces for the specified Ethernet bond interface.

func SCBondInterfaceGetOptions(SCBondInterface) -> CFDictionary?

Returns the configuration settings associated with the specified Ethernet bond interface.

func SCBondInterfaceRemove(SCBondInterface) -> Bool

Removes the Ethernet bond interface from the configuration.

func SCBondInterfaceSetMemberInterfaces(SCBondInterface, CFArray) -> Bool

Sets the member interfaces for the specified Ethernet bond interface.

func SCBondInterfaceSetOptions(SCBondInterface, CFDictionary) -> Bool

Sets the configuration settings for the specified Ethernet bond interface.

func SCBondStatusGetInterfaceStatus(SCBondStatus, SCNetworkInterface?) -> CFDictionary?

Returns the status of the specified member interface of an Ethernet bond or the status of the bond as a whole.

func SCBondStatusGetMemberInterfaces(SCBondStatus) -> CFArray?

Returns the member interfaces that are represented with the Ethernet bond interface.

func SCBondStatusGetTypeID() -> CFTypeID

Returns the type identifier of all `SCBondStatusRef` instances.

