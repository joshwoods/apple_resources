

- CloudKit
- CKSyncEngine
- 
  - CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.AccountChange
- CKSyncEngine.Event.AccountChange.ChangeType
-  CKSyncEngine.Event.AccountChange.ChangeType.signOut(previousUser:) 

Case

# CKSyncEngine.Event.AccountChange.ChangeType.signOut(previousUser:)

A change indicating a sign-out of an iCloud account.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case signOut(previousUser: CKRecord.ID)
```

## Discussion

After the device signs out of the iCloud account, delete any locally stored data that belongs to that account.

## See Also

### Account change types

case signIn(currentUser: CKRecord.ID)

A change indicating a sign-in to an iCloud account.

case switchAccounts(previousUser: CKRecord.ID, currentUser: CKRecord.ID)

A change indicating a switch between two iCloud accounts.

