

- System Configuration
-  SCPreferencesAddValue(\_:\_:\_:) 

Function

# SCPreferencesAddValue(\_:\_:\_:)

Associates the specified value with the specified preference key.

macOS 10.1+

``` source
func SCPreferencesAddValue(
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

true if the value was added; false if the key already exists or if an error occurred.

## Discussion

To commit these changes to permanent storage, you must call SCPreferencesCommitChanges(_:).

## See Also

### Adding, Getting, and Removing Values

func SCPreferencesGetValue(SCPreferences, CFString) -> CFPropertyList?

Retrieves the value associated with the specified preference key.

func SCPreferencesSetValue(SCPreferences, CFString, CFPropertyList) -> Bool

Updates the data associated with the specified preference key with the specified value.

func SCPreferencesRemoveValue(SCPreferences, CFString) -> Bool

Removes the data associated with the specified preference key.

