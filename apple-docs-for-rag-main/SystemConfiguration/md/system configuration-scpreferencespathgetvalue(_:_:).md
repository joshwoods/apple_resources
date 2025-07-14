

- System Configuration
-  SCPreferencesPathGetValue(\_:\_:) 

Function

# SCPreferencesPathGetValue(\_:\_:)

Returns the dictionary associated with the specified path.

macOS 10.1+

``` source
func SCPreferencesPathGetValue(
    _ prefs: SCPreferences,
    _ path: CFString
) -> CFDictionary?
```

## Parameters 

`prefs`  

The preferences session.

`path`  

The path.

## Return Value

The dictionary associated with the specified path, or `NULL` if the path does not exist.

## See Also

### Getting or Removing Information Associated with a Path

func SCPreferencesPathGetLink(SCPreferences, CFString) -> CFString?

Returns the link associated with the specified path.

func SCPreferencesPathRemoveValue(SCPreferences, CFString) -> Bool

Removes the data associated with the specified path.

