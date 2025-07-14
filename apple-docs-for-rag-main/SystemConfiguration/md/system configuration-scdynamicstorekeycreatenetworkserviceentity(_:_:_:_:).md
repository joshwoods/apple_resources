

- System Configuration
-  SCDynamicStoreKeyCreateNetworkServiceEntity(\_:\_:\_:\_:) 

Function

# SCDynamicStoreKeyCreateNetworkServiceEntity(\_:\_:\_:\_:)

Creates a dynamic store key that can be used to access the per-service network configuration information.

macOS 10.1+

``` source
func SCDynamicStoreKeyCreateNetworkServiceEntity(
    _ allocator: CFAllocator?,
    _ domain: CFString,
    _ serviceID: CFString,
    _ entity: CFString?
) -> CFString
```

## Parameters 

`allocator`  

The allocator that should be used to allocate memory for this key. This parameter may be `NULL` in which case the current default allocator is used. If this value is not a valid CFAllocator, the behavior is undefined.

`domain`  

The desired domain, such as the requested configuration or the current state.

`serviceID`  

The service ID or a regular expression pattern.

`entity`  

The specific global entity, such as IPv4 or DNS.

## See Also

### Group

func SCDynamicStoreKeyCreateNetworkGlobalEntity(CFAllocator?, CFString, CFString) -> CFString

Creates a dynamic store key that can be used to access a specific global (as opposed to a per-service or per-interface) network configuration entity.

func SCDynamicStoreKeyCreateNetworkInterface(CFAllocator?, CFString) -> CFString

Creates a dynamic store key that can be used to access the network interface configuration information in the dynamic store.

func SCDynamicStoreKeyCreateNetworkInterfaceEntity(CFAllocator?, CFString, CFString, CFString?) -> CFString

Creates a dynamic store key that can be used to access the per-interface network configuration information in the dynamic store.

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

