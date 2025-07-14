

- SwiftData
- ModelContainer
-  deleteAllData() 

Instance Method

# deleteAllData()

Removes all persisted model data from the app’s persistent storage.

iOS 17.0–18.4DeprecatediPadOS 17.0–18.4DeprecatedMac Catalyst 17.0–18.4DeprecatedmacOS 14.0–15.4DeprecatedtvOS 17.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 10.0–11.4DeprecatedSwift 5.9+

``` source
func deleteAllData()
```

## Discussion

Warning

After you call this method, the container immediately deletes all data from the app’s persistent storage. This deletion is permanent and cannot be undone.

