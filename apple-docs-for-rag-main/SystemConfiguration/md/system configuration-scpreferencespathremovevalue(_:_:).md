

- System Configuration
-  SCPreferencesPathRemoveValue(\_:\_:) 

Function

# SCPreferencesPathRemoveValue(\_:\_:)

Removes the data associated with the specified path.

macOS 10.1+

``` source
func SCPreferencesPathRemoveValue(
    _ prefs: SCPreferences,
    _ path: CFString
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`path`  

The path.

## Return Value

`TRUE` if successful; otherwise, `FALSE`.

## See Also

### Getting or Removing Information Associated with a Path

func SCPreferencesPathGetValue(SCPreferences, CFString) -> CFDictionary?

Returns the dictionary associated with the specified path.

func SCPreferencesPathGetLink(SCPreferences, CFString) -> CFString?

Returns the link associated with the specified path.

