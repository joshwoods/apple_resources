

- System Configuration
-  SCDynamicStoreCopyComputerName(\_:\_:) 

Function

# SCDynamicStoreCopyComputerName(\_:\_:)

Returns the current computer name.

macOS 10.1+

``` source
func SCDynamicStoreCopyComputerName(
    _ store: SCDynamicStore?,
    _ nameEncoding: UnsafeMutablePointer?
) -> CFString?
```

## Parameters 

`store`  

The dynamic store session that should be used for communication with the server. Pass `NULL` to use a temporary session.

`nameEncoding`  

A pointer to memory that, on output, is filled with the encoding associated with the computer or host name, if it is non-`NULL`.

## Return Value

The current computer name, or `NULL` if the name has not been set or if an error occurred. You must release the return value.

## See Also

### Group

func SCDynamicStoreCopyConsoleUser(SCDynamicStore?, UnsafeMutablePointer&lt;uid_t>?, UnsafeMutablePointer&lt;gid_t>?) -> CFString?

Returns information about the user currently logged into the system.

func SCDynamicStoreCopyLocalHostName(SCDynamicStore?) -> CFString?

Returns the current local host name.

func SCDynamicStoreCopyLocation(SCDynamicStore?) -> CFString?

Returns the current location identifier.

func SCDynamicStoreCopyProxies(SCDynamicStore?) -> CFDictionary?

Returns the key-value pairs that represent the current internet proxy settings.

