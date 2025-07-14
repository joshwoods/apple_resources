

- System Configuration
-  SCDynamicStoreCopyLocation(\_:) 

Function

# SCDynamicStoreCopyLocation(\_:)

Returns the current location identifier.

macOS 10.1+

``` source
func SCDynamicStoreCopyLocation(_ store: SCDynamicStore?) -> CFString?
```

## Parameters 

`store`  

The dynamic store session that should be used for communication with the server. Pass `NULL` to use a temporary session.

## Return Value

Returns the current location identifier, or `NULL` if no location identifier has been defined or if an error occurred. You must release the returned value.

## See Also

### Group

func SCDynamicStoreCopyComputerName(SCDynamicStore?, UnsafeMutablePointer&lt;CFStringEncoding>?) -> CFString?

Returns the current computer name.

func SCDynamicStoreCopyConsoleUser(SCDynamicStore?, UnsafeMutablePointer&lt;uid_t>?, UnsafeMutablePointer&lt;gid_t>?) -> CFString?

Returns information about the user currently logged into the system.

func SCDynamicStoreCopyLocalHostName(SCDynamicStore?) -> CFString?

Returns the current local host name.

func SCDynamicStoreCopyProxies(SCDynamicStore?) -> CFDictionary?

Returns the key-value pairs that represent the current internet proxy settings.

