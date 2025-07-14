

- CloudKit
- CKSyncEngine
- 
  - CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.AccountChange
- CKSyncEngine.Event.AccountChange.ChangeType
-  CKSyncEngine.Event.AccountChange.ChangeType.signIn(currentUser:) 

Case

# CKSyncEngine.Event.AccountChange.ChangeType.signIn(currentUser:)

A change indicating a sign-in to an iCloud account.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case signIn(currentUser: CKRecord.ID)
```

## Discussion

If your app has locally stored data when CKSyncEngine notifies it about the device signing in to an iCloud account, perform one of the following actions:

- Keep the local data separate from any remote data

- Merge the local data with the account’s remote data

- Delete the local data

- Prompt the account’s owner to make the decision

## See Also

### Account change types

case signOut(previousUser: CKRecord.ID)

A change indicating a sign-out of an iCloud account.

case switchAccounts(previousUser: CKRecord.ID, currentUser: CKRecord.ID)

A change indicating a switch between two iCloud accounts.

