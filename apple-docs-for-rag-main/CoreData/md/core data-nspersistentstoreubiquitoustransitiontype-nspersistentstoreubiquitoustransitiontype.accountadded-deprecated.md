

- Core Data
- NSPersistentStoreUbiquitousTransitionType
-  NSPersistentStoreUbiquitousTransitionType.accountAdded Deprecated

Case

# NSPersistentStoreUbiquitousTransitionType.accountAdded

This value indicates that a new iCloud account is available, and the persistent store in use will or did transition to the new account.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
case accountAdded
```

Deprecated

Please see the release notes and Core Data documentation.

## Discussion

It is only possible to discern this state when the application is running, and therefore this transition type will only be posted if the account changes while the application is running or in the background.

## See Also

### Constants

case accountRemoved

This value indicates that no iCloud account is available, and the persistent store in use will or did transition to the “local” store.

Deprecated

case contentRemoved

This value indicates that the user has wiped the contents of the iCloud account, usually using Delete All from Documents & Data in Settings.

Deprecated

case initialImportCompleted

This value indicates that the Core Data integration has finished building a store file that is consistent with the contents of the iCloud account, and is ready to replace the fallback store with that file.

Deprecated

