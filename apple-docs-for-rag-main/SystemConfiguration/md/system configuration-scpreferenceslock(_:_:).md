

- System Configuration
-  SCPreferencesLock(\_:\_:) 

Function

# SCPreferencesLock(\_:\_:)

Locks access to the configuration preferences.

macOS 10.1+

``` source
func SCPreferencesLock(
    _ prefs: SCPreferences,
    _ wait: Bool
) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

`wait`  

A Boolean value indicating whether the calling process should block, waiting for another process to complete its update operation and release its lock.

## Return Value

`TRUE` if the lock was obtained; `FALSE` if an error occurred.

## Discussion

This function obtains exclusive access to the configuration preferences. Clients attempting to obtain exclusive access to the preferences either receive a kSCStatusPrefsBusy error or they block, waiting for the lock to be released.

## See Also

### Managing Access to a Preferences Session

func SCPreferencesUnlock(SCPreferences) -> Bool

Releases exclusive access to the configuration preferences.

