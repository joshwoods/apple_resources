

- System Configuration
-  SCBondStatusGetInterfaceStatus(\_:\_:) 

Function

# SCBondStatusGetInterfaceStatus(\_:\_:)

Returns the status of the specified member interface of an Ethernet bond or the status of the bond as a whole.

macOS 10.5+

``` source
func SCBondStatusGetInterfaceStatus(
    _ bondStatus: SCBondStatus,
    _ interface: SCNetworkInterface?
) -> CFDictionary?
```

## Parameters 

`bondStatus`  

The Ethernet bond status.

`interface`  

The member interface whose status is needed. Pass `NULL` to get the status of the Ethernet bond.

## Return Value

The interface status.

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

func SCBondInterfaceSetLocalizedDisplayName(SCBondInterface, CFString) -> Bool

Sets the localized display name for the specified Ethernet bond interface.

func SCBondInterfaceSetMemberInterfaces(SCBondInterface, CFArray) -> Bool

Sets the member interfaces for the specified Ethernet bond interface.

func SCBondInterfaceSetOptions(SCBondInterface, CFDictionary) -> Bool

Sets the configuration settings for the specified Ethernet bond interface.

func SCBondStatusGetMemberInterfaces(SCBondStatus) -> CFArray?

Returns the member interfaces that are represented with the Ethernet bond interface.

func SCBondStatusGetTypeID() -> CFTypeID

Returns the type identifier of all `SCBondStatusRef` instances.

