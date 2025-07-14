

- System Configuration
-  SCPreferencesSetLocalHostName(\_:\_:) 

Function

# SCPreferencesSetLocalHostName(\_:\_:)

Sets the local host name to the specified name.

macOS 10.2+

``` source
func SCPreferencesSetLocalHostName(
    _ prefs: SCPreferences,
    _ name: CFString?
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`name`  

The local host name. This string must conform to the naming conventions of a DNS host name as specified in RFC 1034 (section 3.5).

## Return Value

`TRUE` if successful; otherwise, `FALSE`.

## Discussion

To commit these changes to permanent storage you must call the SCPreferencesCommitChanges(_:) function. In addition, you must call the SCPreferencesApplyChanges(_:) function for the new name to become active.

## See Also

### Setting Configuration Information

func SCPreferencesSetComputerName(SCPreferences, CFString?, CFStringEncoding) -> Bool

Sets the computer name preference to the specified name.

