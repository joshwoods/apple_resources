

- System Configuration
-  SCPreferencesSetComputerName(\_:\_:\_:) 

Function

# SCPreferencesSetComputerName(\_:\_:\_:)

Sets the computer name preference to the specified name.

macOS 10.1+

``` source
func SCPreferencesSetComputerName(
    _ prefs: SCPreferences,
    _ name: CFString?,
    _ nameEncoding: CFStringEncoding
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`name`  

The computer name.

`nameEncoding`  

The encoding associated with the computer name.

## Return Value

`TRUE` if successful; otherwise, `FALSE`.

## Discussion

To commit these changes to permanent storage you must call the SCPreferencesCommitChanges(_:) function. In addition, you must call the SCPreferencesApplyChanges(_:) function for the new name to become active.

## See Also

### Setting Configuration Information

func SCPreferencesSetLocalHostName(SCPreferences, CFString?) -> Bool

Sets the local host name to the specified name.

