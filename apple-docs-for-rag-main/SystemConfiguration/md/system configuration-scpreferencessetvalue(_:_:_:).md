

- System Configuration
-  SCPreferencesSetValue(\_:\_:\_:) 

Function

# SCPreferencesSetValue(\_:\_:\_:)

Updates the data associated with the specified preference key with the specified value.

macOS 10.1+

``` source
func SCPreferencesSetValue(
    _ prefs: SCPreferences,
    _ key: CFString,
    _ value: CFPropertyList
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`key`  

The preference key.

`value`  

The value to associate with the preference key.

## Return Value

`TRUE` if the value was set; `FALSE` if an error occurred.

## Discussion

This function adds or replaces the value associated with the specified key. To commit these changes to permanent storage you must call SCPreferencesCommitChanges(_:).

## See Also

### Adding, Getting, and Removing Values

func SCPreferencesAddValue(SCPreferences, CFString, CFPropertyList) -> Bool

Associates the specified value with the specified preference key.

func SCPreferencesGetValue(SCPreferences, CFString) -> CFPropertyList?

Retrieves the value associated with the specified preference key.

func SCPreferencesRemoveValue(SCPreferences, CFString) -> Bool

Removes the data associated with the specified preference key.

