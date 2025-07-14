

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.AccountChange
-  CKSyncEngine.Event.AccountChange.ChangeType 

Enumeration

# CKSyncEngine.Event.AccountChange.ChangeType

Describes a change to the device’s iCloud account.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
enum ChangeType
```

## Topics

### Account change types

case signIn(currentUser: CKRecord.ID)

A change indicating a sign-in to an iCloud account.

case signOut(previousUser: CKRecord.ID)

A change indicating a sign-out of an iCloud account.

case switchAccounts(previousUser: CKRecord.ID, currentUser: CKRecord.ID)

A change indicating a switch between two iCloud accounts.

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

## See Also

### Understanding the change

let changeType: CKSyncEngine.Event.AccountChange.ChangeType

The iCloud account’s change type.

enum CKSyncEngineAccountChangeType

Describes a change to the device’s iCloud account.

