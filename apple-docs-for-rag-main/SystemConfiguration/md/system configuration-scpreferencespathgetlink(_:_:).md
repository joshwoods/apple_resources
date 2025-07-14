

- System Configuration
-  SCPreferencesPathGetLink(\_:\_:) 

Function

# SCPreferencesPathGetLink(\_:\_:)

Returns the link associated with the specified path.

macOS 10.1+

``` source
func SCPreferencesPathGetLink(
    _ prefs: SCPreferences,
    _ path: CFString
) -> CFString?
```

## Parameters 

`prefs`  

The preferences session.

`path`  

The path.

## Return Value

The link associated with the specified path, or `NULL` if the path is not a link or does not exist.

## See Also

### Getting or Removing Information Associated with a Path

func SCPreferencesPathGetValue(SCPreferences, CFString) -> CFDictionary?

Returns the dictionary associated with the specified path.

func SCPreferencesPathRemoveValue(SCPreferences, CFString) -> Bool

Removes the data associated with the specified path.

