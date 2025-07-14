

- System Configuration
-  SCNetworkConfiguration 

API Collection

# SCNetworkConfiguration

## Overview

The `SCNetworkConfiguration` programming interface provides access to the stored network configuration. The functions include providing access to the network-capable devices on the system, the network sets, network services, and network protocols. Note that these functions follow Core Foundation function-name conventions. A function that has “Create” or “Copy” in its name returns a reference you must release with the CFRelease function.

Note that when using the functions in this programming interface, you must call the SCPreferencesCommitChanges(_:) function to ensure that your changes are committed to permanent storage.

## Topics

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

func SCBondStatusGetInterfaceStatus(SCBondStatus, SCNetworkInterface?) -> CFDictionary?

Returns the status of the specified member interface of an Ethernet bond or the status of the bond as a whole.

func SCBondStatusGetMemberInterfaces(SCBondStatus) -> CFArray?

Returns the member interfaces that are represented with the Ethernet bond interface.

func SCBondStatusGetTypeID() -> CFTypeID

Returns the type identifier of all `SCBondStatusRef` instances.

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

func SCNetworkInterfaceGetSupportedProtocolTypes(SCNetworkInterface) -> CFArray?

Identifies all of the network protocol types, such as IPv4 and IPv6, that can be layered on top of the specified interface.

func SCNetworkInterfaceGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkInterface` instances.

func SCNetworkInterfaceSetConfiguration(SCNetworkInterface, CFDictionary?) -> Bool

Stores the configuration settings for the specified interface.

func SCNetworkInterfaceSetExtendedConfiguration(SCNetworkInterface, CFString, CFDictionary?) -> Bool

Stores the extended configuration settings for the specified interface.

func SCNetworkInterfaceSetMTU(SCNetworkInterface, Int32) -> Bool

Sets the requested MTU setting for the specified network interface.

func SCNetworkInterfaceSetMediaOptions(SCNetworkInterface, CFString?, CFArray?) -> Bool

Sets the requested media subtype and options for the specified network interface.

### Configuring Network Protocols

func SCNetworkProtocolGetConfiguration(SCNetworkProtocol) -> CFDictionary?

Returns the configuration settings associated with the specified protocol.

func SCNetworkProtocolGetEnabled(SCNetworkProtocol) -> Bool

Returns a Boolean value indicating whether the specified protocol is enabled.

func SCNetworkProtocolGetProtocolType(SCNetworkProtocol) -> CFString?

Returns the type of the specified network protocol.

func SCNetworkProtocolGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkProtocol` instances.

func SCNetworkProtocolSetConfiguration(SCNetworkProtocol, CFDictionary?) -> Bool

Stores the configuration settings for the specified network protocol.

func SCNetworkProtocolSetEnabled(SCNetworkProtocol, Bool) -> Bool

Enables or disables the specified protocol.

### Configuring Network Services

func SCNetworkServiceAddProtocolType(SCNetworkService, CFString) -> Bool

Adds the network protocol of the specified type to the specified service.

func SCNetworkServiceCopy(SCPreferences, CFString) -> SCNetworkService?

Returns the network service with the specified identifier.

func SCNetworkServiceCopyAll(SCPreferences) -> CFArray?

Returns all available network services for the specified preferences.

func SCNetworkServiceCopyProtocol(SCNetworkService, CFString) -> SCNetworkProtocol?

Returns the network protocol of the specified type for the specified service.

func SCNetworkServiceCopyProtocols(SCNetworkService) -> CFArray?

Returns all network protocols associated with the specified service.

func SCNetworkServiceCreate(SCPreferences, SCNetworkInterface) -> SCNetworkService?

Creates a new network service for the specified interface in the configuration.

func SCNetworkServiceEstablishDefaultConfiguration(SCNetworkService) -> Bool

Establishes the default configuration for the specified network service.

func SCNetworkServiceGetEnabled(SCNetworkService) -> Bool

Returns a Boolean value indicating whether the specified service is enabled.

func SCNetworkServiceGetInterface(SCNetworkService) -> SCNetworkInterface?

Returns the network interface associated with the specified service.

func SCNetworkServiceGetName(SCNetworkService) -> CFString?

Returns the user-specified name associated with the specified service.

func SCNetworkServiceGetServiceID(SCNetworkService) -> CFString?

Returns the identifier for the specified service.

func SCNetworkServiceGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkService` instances.

func SCNetworkServiceRemove(SCNetworkService) -> Bool

Removes the specified network service from the configuration.

func SCNetworkServiceRemoveProtocolType(SCNetworkService, CFString) -> Bool

Removes the network protocol of the specified type from the specified service.

func SCNetworkServiceSetEnabled(SCNetworkService, Bool) -> Bool

Enables or disables the specified service.

func SCNetworkServiceSetName(SCNetworkService, CFString?) -> Bool

Stores the user-specified name for the specified service.

### Configuring Network Sets

func SCNetworkSetAddService(SCNetworkSet, SCNetworkService) -> Bool

Adds the specified network service to the specified set.

func SCNetworkSetContainsInterface(SCNetworkSet, SCNetworkInterface) -> Bool

Returns a Boolean value indicating whether the specified interface is represented by at least one network service in the specified set.

func SCNetworkSetCopy(SCPreferences, CFString) -> SCNetworkSet?

Returns the set with the specified identifier.

func SCNetworkSetCopyAll(SCPreferences) -> CFArray?

Returns all available sets for the specified preferences session.

func SCNetworkSetCopyCurrent(SCPreferences) -> SCNetworkSet?

Returns the current set.

func SCNetworkSetCopyServices(SCNetworkSet) -> CFArray?

Returns all network services associated with the specified set.

func SCNetworkSetCreate(SCPreferences) -> SCNetworkSet?

Creates a new set in the configuration.

func SCNetworkSetGetName(SCNetworkSet) -> CFString?

Returns the user-specified name associated with the specified set.

func SCNetworkSetGetServiceOrder(SCNetworkSet) -> CFArray?

Returns the user-specified ordering of network services within the specified set.

func SCNetworkSetGetSetID(SCNetworkSet) -> CFString?

Returns the identifier for the specified set.

func SCNetworkSetGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkSet` instances.

func SCNetworkSetRemove(SCNetworkSet) -> Bool

Removes the specified set from the configuration.

func SCNetworkSetRemoveService(SCNetworkSet, SCNetworkService) -> Bool

Removes the specified network service from the specified set.

func SCNetworkSetSetCurrent(SCNetworkSet) -> Bool

Specifies the set that should be the current set.

func SCNetworkSetSetName(SCNetworkSet, CFString?) -> Bool

Stores the user-specified name for the specified set.

func SCNetworkSetSetServiceOrder(SCNetworkSet, CFArray) -> Bool

Stores the user-specified ordering of network services for the specified set.

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

func SCVLANInterfaceSetPhysicalInterfaceAndTag(SCVLANInterface, SCNetworkInterface, CFNumber) -> Bool

Updates the specified virtual LAN (VLAN) interface with the specified information.

### Data Types

class SCNetworkInterface

The reference to an object that represents a network interface.

typealias SCBondInterface

The reference to an object that represents an Ethernet bond interface.

class SCBondStatus

The reference to an object that represents the status of an Ethernet bond interface.

typealias SCVLANInterface

The reference to an object that represents a virtual LAN (VLAN) interface.

class SCNetworkProtocol

The reference to an object that represents a network protocol.

class SCNetworkService

The reference to an object that represents a network service.

class SCNetworkSet

The reference to an object that represents a network set.

### Constants

Ethernet Bond Aggregation Status

Ethernet bond aggregation status codes.

Ethernet Bond Status Constants

Ethernet bond status codes.

Network Interface Types

Keys that identify network interface types.

Network Protocol Types

Keys that identify network protocol types.

## See Also

### Reference

SCDynamicStore

SCDynamicStoreCopySpecific

SCDynamicStoreKey

SCNetwork

SCNetworkConnection

SCNetworkReachability

SCPreferences

SCPreferencesPath

SCPreferencesSetSpecific

SCSchemaDefinitions

System Configuration

SystemConfiguration Enumerations

SystemConfiguration Constants

SystemConfiguration Functions

SystemConfiguration Data Types

