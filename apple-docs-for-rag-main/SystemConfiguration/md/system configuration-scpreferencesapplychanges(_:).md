

- System Configuration
-  SCPreferencesApplyChanges(\_:) 

Function

# SCPreferencesApplyChanges(\_:)

Requests that the currently stored configuration preferences be applied to the active configuration.

macOS 10.1+

``` source
func SCPreferencesApplyChanges(_ prefs: SCPreferences) -> Bool
```

## Parameters 

`prefs`  

The preferences session.

## Return Value

`TRUE` if the lock was obtained; `FALSE` if an error occurred.

## See Also

### Applying and Committing Changes

func SCPreferencesCommitChanges(SCPreferences) -> Bool

Commits changes made to the configuration preferences to persistent storage.

func SCPreferencesSynchronize(SCPreferences)

Synchronizes accessed preferences with committed changes.

