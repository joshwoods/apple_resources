

- Core Data
- NSPersistentStoreUbiquitousTransitionType
-  NSPersistentStoreUbiquitousTransitionType.initialImportCompleted Deprecated

Case

# NSPersistentStoreUbiquitousTransitionType.initialImportCompleted

This value indicates that the Core Data integration has finished building a store file that is consistent with the contents of the iCloud account, and is ready to replace the fallback store with that file.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
case initialImportCompleted
```

Deprecated

Please see the release notes and Core Data documentation.

## See Also

### Constants

case accountAdded

This value indicates that a new iCloud account is available, and the persistent store in use will or did transition to the new account.

Deprecated

case accountRemoved

This value indicates that no iCloud account is available, and the persistent store in use will or did transition to the “local” store.

Deprecated

case contentRemoved

This value indicates that the user has wiped the contents of the iCloud account, usually using Delete All from Documents & Data in Settings.

Deprecated

