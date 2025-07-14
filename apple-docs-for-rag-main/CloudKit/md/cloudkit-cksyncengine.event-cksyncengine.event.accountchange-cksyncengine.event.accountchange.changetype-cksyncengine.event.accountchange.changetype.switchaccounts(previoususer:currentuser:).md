

- CloudKit
- CKSyncEngine
- 
  - CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.AccountChange
- CKSyncEngine.Event.AccountChange.ChangeType
-  CKSyncEngine.Event.AccountChange.ChangeType.switchAccounts(previousUser:currentUser:) 

Case

# CKSyncEngine.Event.AccountChange.ChangeType.switchAccounts(previousUser:currentUser:)

A change indicating a switch between two iCloud accounts.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case switchAccounts(
    previousUser: CKRecord.ID,
    currentUser: CKRecord.ID
)
```

## Discussion

If the device changes iCloud accounts while your app isn’t running, CKSyncEngine notifies it about that change when the app next launches. Make sure to delete any locally stored data belonging to the `previousUser` account.

## See Also

### Account change types

case signIn(currentUser: CKRecord.ID)

A change indicating a sign-in to an iCloud account.

case signOut(previousUser: CKRecord.ID)

A change indicating a sign-out of an iCloud account.

