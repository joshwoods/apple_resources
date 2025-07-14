

- System Configuration
-  SCPreferencesGetValue(\_:\_:) 

Function

# SCPreferencesGetValue(\_:\_:)

Retrieves the value associated with the specified preference key.

macOS 10.1+

``` source
func SCPreferencesGetValue(
    _ prefs: SCPreferences,
    _ key: CFString
) -> CFPropertyList?
```

## Parameters 

`prefs`  

The preferences session.

`key`  

The preference key.

## Return Value

The value associated with the specified preference key (can be `NULL` if no value exists).

## Discussion

To avoid inadvertantly reading stale data, first call SCPreferencesLock(_:_:) before calling this function.

## See Also

### Adding, Getting, and Removing Values

func SCPreferencesAddValue(SCPreferences, CFString, CFPropertyList) -> Bool

Associates the specified value with the specified preference key.

func SCPreferencesSetValue(SCPreferences, CFString, CFPropertyList) -> Bool

Updates the data associated with the specified preference key with the specified value.

func SCPreferencesRemoveValue(SCPreferences, CFString) -> Bool

Removes the data associated with the specified preference key.

