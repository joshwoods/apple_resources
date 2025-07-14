

- System Configuration
-  SCDynamicStoreKey 

API Collection

# SCDynamicStoreKey

## Overview

The `SCDynamicStoreKey` programming interface provides convenience functions that an application can use to create a correctly formatted dynamic store key for accessing specific items in the dynamic store. An application can then use the resulting string in any function that requires a dynamic store key.

## Topics

### Group

func SCDynamicStoreKeyCreateNetworkGlobalEntity(CFAllocator?, CFString, CFString) -> CFString

Creates a dynamic store key that can be used to access a specific global (as opposed to a per-service or per-interface) network configuration entity.

func SCDynamicStoreKeyCreateNetworkInterface(CFAllocator?, CFString) -> CFString

Creates a dynamic store key that can be used to access the network interface configuration information in the dynamic store.

func SCDynamicStoreKeyCreateNetworkInterfaceEntity(CFAllocator?, CFString, CFString, CFString?) -> CFString

Creates a dynamic store key that can be used to access the per-interface network configuration information in the dynamic store.

func SCDynamicStoreKeyCreateNetworkServiceEntity(CFAllocator?, CFString, CFString, CFString?) -> CFString

Creates a dynamic store key that can be used to access the per-service network configuration information.

func SCDynamicStoreKeyCreateComputerName(CFAllocator?) -> CFString

Creates a key that can be used to receive notifications when the current computer name changes.

func SCDynamicStoreKeyCreateConsoleUser(CFAllocator?) -> CFString

Creates a key that can be used to receive notifications when the current console user changes.

func SCDynamicStoreKeyCreateHostNames(CFAllocator?) -> CFString

Creates a key that can be used to receive notifications when the `HostNames` entity changes.

func SCDynamicStoreKeyCreateLocation(CFAllocator?) -> CFString

Creates a key that can be used to receive notifications when the location identifier changes.

func SCDynamicStoreKeyCreateProxies(CFAllocator?) -> CFString

Creates a key that can be used to receive notifications when the current network proxy settings are changed.

## See Also

### Reference

SCDynamicStore

SCDynamicStoreCopySpecific

SCNetwork

SCNetworkConfiguration

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

