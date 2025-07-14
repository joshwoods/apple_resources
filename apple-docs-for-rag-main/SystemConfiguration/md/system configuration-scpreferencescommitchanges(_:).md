

- System Configuration
-  SCPreferencesCommitChanges(\_:) 

Function

# SCPreferencesCommitChanges(\_:)

Commits changes made to the configuration preferences to persistent storage.

macOS 10.1+

``` source
func SCPreferencesCommitChanges(_ prefs: SCPreferences) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

## Return Value

`TRUE` if the lock was obtained; `FALSE` if an error occurred.

## Discussion

Implicit calls to the SCPreferencesLock(_:_:) and SCPreferencesUnlock(_:) functions are made if exclusive access has not already been established.

Note

This function commits changes to persistent storage. To apply the changes to the running system, use the SCPreferencesApplyChanges(_:) function.

## See Also

### Applying and Committing Changes

func SCPreferencesApplyChanges(SCPreferences) -> Bool

Requests that the currently stored configuration preferences be applied to the active configuration.

func SCPreferencesSynchronize(SCPreferences)

Synchronizes accessed preferences with committed changes.

