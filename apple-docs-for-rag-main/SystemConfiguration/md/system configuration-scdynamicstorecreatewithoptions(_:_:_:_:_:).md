

- System Configuration
-  SCDynamicStoreCreateWithOptions(\_:\_:\_:\_:\_:) 

Function

# SCDynamicStoreCreateWithOptions(\_:\_:\_:\_:\_:)

Creates a new session used to interact with the dynamic store maintained by the System Configuration server.

macOS 10.4+

``` source
func SCDynamicStoreCreateWithOptions(
    _ allocator: CFAllocator?,
    _ name: CFString,
    _ storeOptions: CFDictionary?,
    _ callout: SCDynamicStoreCallBack?,
    _ context: UnsafeMutablePointer?
) -> SCDynamicStore?
```

## Parameters 

`allocator`  

The allocator that should be used to allocate memory for the local dynamic store object. This parameter may be `NULL` in which case the current default allocator is used. If this value is not a valid CFAllocator, the behavior is undefined.

`name`  

The name of the calling process or plug-in of the caller.

`storeOptions`  

A dictionary of options for the dynamic store session (such as whether all keys added or set into the dynamic store should be per-session keys). Pass `NULL` if no options are desired.

Currently, the available options are:

| Key | Value |
|----|----|
| kSCDynamicStoreUseSessionKeys | `CFBooleanRef` |

`callout`  

The function to be called when a watched value in the dynamic store is changed. Pass `NULL` if no callouts are desired.

`context`  

The context associated with the callout. See SCDynamicStoreContext for more information about this value.

## Return Value

A reference to the new dynamic store session. You must release the returned value.

## See Also

### Creating a Dynamic Store Session

func SCDynamicStoreCreate(CFAllocator?, CFString, SCDynamicStoreCallBack?, UnsafeMutablePointer&lt;SCDynamicStoreContext>?) -> SCDynamicStore?

Creates a new session used to interact with the dynamic store maintained by the System Configuration server.

