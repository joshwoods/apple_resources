

- System Configuration
-  SCPreferencesPathCreateUniqueChild(\_:\_:) 

Function

# SCPreferencesPathCreateUniqueChild(\_:\_:)

Creates a new path component rooted at the specified path in the dictionary hierarchy.

macOS 10.1+

``` source
func SCPreferencesPathCreateUniqueChild(
    _ prefs: SCPreferences,
    _ prefix: CFString
) -> CFString?
```

## Parameters 

`prefs`  

The preferences session.

`prefix`  

The parent path.

## Return Value

A string representing the new (unique) child path, or `NULL` if the specified path does not exist.

