

- System Configuration
-  SCPreferencesCreate(\_:\_:\_:) 

Function

# SCPreferencesCreate(\_:\_:\_:)

Initiates access to the per-system set of configuration preferences.

macOS 10.1+

``` source
func SCPreferencesCreate(
    _ allocator: CFAllocator?,
    _ name: CFString,
    _ prefsID: CFString?
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

## Return Value

A reference to the new preferences session. You must release the returned value.

## See Also

### Creating a Preferences Session

func SCPreferencesCreateWithAuthorization(CFAllocator?, CFString, CFString?, AuthorizationRef?) -> SCPreferences?

Initiates access to the per-system set of configuration preferences with the specified authorization.

