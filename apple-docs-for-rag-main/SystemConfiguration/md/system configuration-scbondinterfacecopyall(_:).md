

- System Configuration
-  SCBondInterfaceCopyAll(\_:) 

Function

# SCBondInterfaceCopyAll(\_:)

Returns all Ethernet bond interfaces on the system.

macOS 10.5+

``` source
func SCBondInterfaceCopyAll(_ prefs: SCPreferences) -> CFArray
```

## Parameters 

`prefs`  

The preferences session.

## Return Value

The list of Ethernet bond interfaces on the system. You must release the returned value.

## See Also

### Configuring Ethernet Bond Interfaces

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

func SCBondStatusGetInterfaceStatus(SCBondStatus, SCNetworkInterface?) -> CFDictionary?

Returns the status of the specified member interface of an Ethernet bond or the status of the bond as a whole.

func SCBondStatusGetMemberInterfaces(SCBondStatus) -> CFArray?

Returns the member interfaces that are represented with the Ethernet bond interface.

func SCBondStatusGetTypeID() -> CFTypeID

Returns the type identifier of all `SCBondStatusRef` instances.

