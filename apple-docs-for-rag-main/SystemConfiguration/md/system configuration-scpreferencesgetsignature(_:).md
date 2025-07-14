

- System Configuration
-  SCPreferencesGetSignature(\_:) 

Function

# SCPreferencesGetSignature(\_:)

Returns a value that can be used to determine if the saved configuration preferences have changed.

macOS 10.1+

``` source
func SCPreferencesGetSignature(_ prefs: SCPreferences) -> CFData?
```

## Parameters 

`prefs`  

The preferences session.

## Return Value

Data that reflects the signature of the configuration preferences at the time of the call to the SCPreferencesCreate(_:_:_:) function.

## See Also

### Getting Information About a Preferences Session

func SCPreferencesGetTypeID() -> CFTypeID

Returns the type identifier of all `SCPreferences` instances.

func SCPreferencesCopyKeyList(SCPreferences) -> CFArray?

Returns the currently defined preference keys.

