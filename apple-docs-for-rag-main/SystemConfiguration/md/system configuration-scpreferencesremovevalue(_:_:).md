

- System Configuration
-  SCPreferencesRemoveValue(\_:\_:) 

Function

# SCPreferencesRemoveValue(\_:\_:)

Removes the data associated with the specified preference key.

macOS 10.1+

``` source
func SCPreferencesRemoveValue(
    _ prefs: SCPreferences,
    _ key: CFString
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`key`  

The preference key.

## Return Value

`TRUE` if the value was removed; `FALSE` if the key does not exist or if an error occurred.

## See Also

### Adding, Getting, and Removing Values

func SCPreferencesAddValue(SCPreferences, CFString, CFPropertyList) -> Bool

Associates the specified value with the specified preference key.

func SCPreferencesGetValue(SCPreferences, CFString) -> CFPropertyList?

Retrieves the value associated with the specified preference key.

func SCPreferencesSetValue(SCPreferences, CFString, CFPropertyList) -> Bool

Updates the data associated with the specified preference key with the specified value.

