

- System Configuration
-  SCPreferencesPathSetLink(\_:\_:\_:) 

Function

# SCPreferencesPathSetLink(\_:\_:\_:)

Associates a link to a second dictionary at the specified path.

macOS 10.1+

``` source
func SCPreferencesPathSetLink(
    _ prefs: SCPreferences,
    _ path: CFString,
    _ link: CFString
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`path`  

The path.

`link`  

The link to be stored at the path.

## Return Value

`TRUE` if successful; otherwise, `FALSE`.

## See Also

### Associating Information with a Path

func SCPreferencesPathSetValue(SCPreferences, CFString, CFDictionary) -> Bool

Associates the specified dictionary with the specified path.

