

- System Configuration
-  SCPreferencesSynchronize(\_:) 

Function

# SCPreferencesSynchronize(\_:)

Synchronizes accessed preferences with committed changes.

macOS 10.4+

``` source
func SCPreferencesSynchronize(_ prefs: SCPreferences)
```

## Parameters 

`prefs`  

The preferences session.

## Discussion

Any references to preference values returned by calls to SCPreferencesGetValue(_:_:) are no longer valid unless they were explicitly retained or copied. Any preference values that were updated (added, set, or removed), but not committed, are discarded.

## See Also

### Applying and Committing Changes

func SCPreferencesApplyChanges(SCPreferences) -> Bool

Requests that the currently stored configuration preferences be applied to the active configuration.

func SCPreferencesCommitChanges(SCPreferences) -> Bool

Commits changes made to the configuration preferences to persistent storage.

