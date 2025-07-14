

- Core Data
-  NSPersistentStoreUbiquitousTransitionType Deprecated

Enumeration

# NSPersistentStoreUbiquitousTransitionType

These constants are used as the value corresponding to the NSPersistentStoreUbiquitousTransitionTypeKey in the user info dictionary of NSPersistentStoreCoordinatorStoresWillChangeNotification and NSPersistentStoreCoordinatorStoresDidChangeNotification notifications to identify the type of event leading to a change.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum NSPersistentStoreUbiquitousTransitionType
```

Deprecated

Please see the release notes and Core Data documentation.

## Topics

### Constants

case accountAdded

This value indicates that a new iCloud account is available, and the persistent store in use will or did transition to the new account.

case accountRemoved

This value indicates that no iCloud account is available, and the persistent store in use will or did transition to the “local” store.

case contentRemoved

This value indicates that the user has wiped the contents of the iCloud account, usually using Delete All from Documents & Data in Settings.

case initialImportCompleted

This value indicates that the Core Data integration has finished building a store file that is consistent with the contents of the iCloud account, and is ready to replace the fallback store with that file.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

