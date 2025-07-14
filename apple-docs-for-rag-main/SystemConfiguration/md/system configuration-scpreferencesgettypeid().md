

- System Configuration
-  SCPreferencesGetTypeID() 

Function

# SCPreferencesGetTypeID()

Returns the type identifier of all `SCPreferences` instances.

macOS 10.1+

``` source
func SCPreferencesGetTypeID() -> CFTypeID
```

## See Also

### Getting Information About a Preferences Session

func SCPreferencesCopyKeyList(SCPreferences) -> CFArray?

Returns the currently defined preference keys.

func SCPreferencesGetSignature(SCPreferences) -> CFData?

Returns a value that can be used to determine if the saved configuration preferences have changed.

