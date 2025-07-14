

- System Configuration
-  SCPreferencesCreateWithAuthorization(\_:\_:\_:\_:) 

Function

# SCPreferencesCreateWithAuthorization(\_:\_:\_:\_:)

Initiates access to the per-system set of configuration preferences with the specified authorization.

macOS 10.5+

``` source
func SCPreferencesCreateWithAuthorization(
    _ allocator: CFAllocator?,
    _ name: CFString,
    _ prefsID: CFString?,
    _ authorization: AuthorizationRef?
) -> SCPreferences?
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for this preferences session. If the value is not a valid `CFAllocator`, the behavior is undefined. Pass `NULL` or kCFAllocatorDefault to use the current default `CFAllocator`.

`name`  

The name of the calling process.

`prefsID`  

The name of the group of preferences to be accessed or updated. A name that starts with a leading “/” character specifies the absolute path to the file containing the preferences to be accessed. A name that does not start with a leading “/” character specifies a file relative to the default system preferences directory.

To access the default system preferences, pass in `NULL`.

`authorization`  

An authorization reference that is used to authorize any access to the enhanced privileges needed to manage the preferences session.

## Return Value

A reference to the new preferences session. You must release the returned value.

## See Also

### Creating a Preferences Session

func SCPreferencesCreate(CFAllocator?, CFString, CFString?) -> SCPreferences?

Initiates access to the per-system set of configuration preferences.

