

- System Configuration
-  SCPreferencesCopyKeyList(\_:) 

Function

# SCPreferencesCopyKeyList(\_:)

Returns the currently defined preference keys.

macOS 10.1+

``` source
func SCPreferencesCopyKeyList(_ prefs: SCPreferences) -> CFArray?
```

## Parameters 

`prefs`  

The preferences session.

## Return Value

An array of currently defined preference keys. You must release the returned value.

## See Also

### Getting Information About a Preferences Session

func SCPreferencesGetTypeID() -> CFTypeID

Returns the type identifier of all `SCPreferences` instances.

func SCPreferencesGetSignature(SCPreferences) -> CFData?

Returns a value that can be used to determine if the saved configuration preferences have changed.

