

- System Configuration
-  SCDynamicStoreCopyLocalHostName(\_:) 

Function

# SCDynamicStoreCopyLocalHostName(\_:)

Returns the current local host name.

macOS 10.1+

``` source
func SCDynamicStoreCopyLocalHostName(_ store: SCDynamicStore?) -> CFString?
```

## Parameters 

`store`  

The dynamic store session that should be used for communication with the server. Pass `NULL` to use a temporary session.

## Return Value

Returns the current local host name, or `NULL` if the name has not been set or if an error occurred. You must release the return value.

## See Also

### Group

func SCDynamicStoreCopyComputerName(SCDynamicStore?, UnsafeMutablePointer&lt;CFStringEncoding>?) -> CFString?

Returns the current computer name.

func SCDynamicStoreCopyConsoleUser(SCDynamicStore?, UnsafeMutablePointer&lt;uid_t>?, UnsafeMutablePointer&lt;gid_t>?) -> CFString?

Returns information about the user currently logged into the system.

func SCDynamicStoreCopyLocation(SCDynamicStore?) -> CFString?

Returns the current location identifier.

func SCDynamicStoreCopyProxies(SCDynamicStore?) -> CFDictionary?

Returns the key-value pairs that represent the current internet proxy settings.

