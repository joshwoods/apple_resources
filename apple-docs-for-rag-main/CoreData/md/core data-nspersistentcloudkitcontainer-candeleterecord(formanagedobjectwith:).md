

- Core Data
- NSPersistentCloudKitContainer
-  canDeleteRecord(forManagedObjectWith:) 

Instance Method

# canDeleteRecord(forManagedObjectWith:)

Returns a Boolean value that indicates whether the user can delete the managed object’s underlying CloudKit record.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func canDeleteRecord(forManagedObjectWith objectID: NSManagedObjectID) -> Bool
```

## Parameters 

`objectID`  

The ID of the managed object.

## Return Value

true if the user can delete the CloudKit record; otherwise, false.

## Discussion

This method returns true if canModifyManagedObjects(in:) returns true and any of the following conditions are true:

- `objectID` is a temporary object identifier.

- The persistent store that contains the managed object isn’t using CloudKit.

- The persistent store manages the user’s private database.

- The persistent store manages the public database, and the user owns the underlying record or Core Data has yet to save the managed object to iCloud.

- The persistent store manages the shared database, and the user has the necessary permissions to delete the managed object’s underlying record. For more information, see CKShare.ParticipantPermission.

## See Also

### Checking Permissions

func canUpdateRecord(forManagedObjectWith: NSManagedObjectID) -> Bool

Returns a Boolean value that indicates whether the user can modify the managed object’s underlying CloudKit record.

func canModifyManagedObjects(in: NSPersistentStore) -> Bool

Returns a Boolean value that indicates whether the user can modify the specified persistent store.

