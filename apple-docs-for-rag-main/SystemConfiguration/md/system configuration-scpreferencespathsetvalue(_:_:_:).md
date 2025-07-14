

- System Configuration
-  SCPreferencesPathSetValue(\_:\_:\_:) 

Function

# SCPreferencesPathSetValue(\_:\_:\_:)

Associates the specified dictionary with the specified path.

macOS 10.1+

``` source
func SCPreferencesPathSetValue(
    _ prefs: SCPreferences,
    _ path: CFString,
    _ value: CFDictionary
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`path`  

The path.

`value`  

The dictionary of data to be stored at the path.

## Return Value

`TRUE` if successful; otherwise, `FALSE`.

## See Also

### Associating Information with a Path

func SCPreferencesPathSetLink(SCPreferences, CFString, CFString) -> Bool

Associates a link to a second dictionary at the specified path.

