

- System Configuration
-  SCDynamicStoreCopyConsoleUser(\_:\_:\_:) 

Function

# SCDynamicStoreCopyConsoleUser(\_:\_:\_:)

Returns information about the user currently logged into the system.

macOS 10.1+

``` source
func SCDynamicStoreCopyConsoleUser(
    _ store: SCDynamicStore?,
    _ uid: UnsafeMutablePointer?,
    _ gid: UnsafeMutablePointer?
) -> CFString?
```

## Parameters 

`store`  

The dynamic store session that should be used for communication with the server. Pass `NULL` to use a temporary session.

`uid`  

A pointer to memory that, on output, is filled with the user ID of the currently logged-in user. If `NULL`, this value is not returned.

`gid`  

A pointer to memory that, on output, is filled with the group ID of the currently logged-in user. If `NULL`, this value is not returned.

## Return Value

Returns the name, user ID, and group ID of the user currently logged into the system, or `NULL` if no user is logged in or if an error occurred. You must release the returned values.

## Discussion

Note that this function only provides information about the primary console. It does not provide any details about console sessions that have fast user switched out or about other consoles.

## See Also

### Group

func SCDynamicStoreCopyComputerName(SCDynamicStore?, UnsafeMutablePointer&lt;CFStringEncoding>?) -> CFString?

Returns the current computer name.

func SCDynamicStoreCopyLocalHostName(SCDynamicStore?) -> CFString?

Returns the current local host name.

func SCDynamicStoreCopyLocation(SCDynamicStore?) -> CFString?

Returns the current location identifier.

func SCDynamicStoreCopyProxies(SCDynamicStore?) -> CFDictionary?

Returns the key-value pairs that represent the current internet proxy settings.

