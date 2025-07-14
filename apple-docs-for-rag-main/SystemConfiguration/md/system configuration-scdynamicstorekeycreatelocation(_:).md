

- System Configuration
-  SCDynamicStoreKeyCreateLocation(\_:) 

Function

# SCDynamicStoreKeyCreateLocation(\_:)

Creates a key that can be used to receive notifications when the location identifier changes.

macOS 10.2+

``` source
func SCDynamicStoreKeyCreateLocation(_ allocator: CFAllocator?) -> CFString
```

## Parameters 

`allocator`  

The allocator that should be used to allocate memory for this key. This parameter may be `NULL` in which case the current default allocator is used. If this value is not a valid CFAllocator, the behavior is undefined.

## Return Value

A notification string for the current location identifier.

## Discussion

Use this key with the SCDynamicStoreSetNotificationKeys(_:_:_:) function.

## See Also

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

func SCDynamicStoreKeyCreateProxies(CFAllocator?) -> CFString

Creates a key that can be used to receive notifications when the current network proxy settings are changed.

