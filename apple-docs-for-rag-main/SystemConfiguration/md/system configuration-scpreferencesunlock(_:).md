

- System Configuration
-  SCPreferencesUnlock(\_:) 

Function

# SCPreferencesUnlock(\_:)

Releases exclusive access to the configuration preferences.

macOS 10.1+

``` source
func SCPreferencesUnlock(_ prefs: SCPreferences) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

## Return Value

`TRUE` if the lock was obtained; `FALSE` if an error occurred.

## Discussion

After exclusive access has been released, other clients can establish exclusive access to the preferences.

## See Also

### Managing Access to a Preferences Session

func SCPreferencesLock(SCPreferences, Bool) -> Bool

Locks access to the configuration preferences.

