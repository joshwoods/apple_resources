

- Core Data
- NSPersistentCloudKitContainer
-  canModifyManagedObjects(in:) 

Instance Method

# canModifyManagedObjects(in:)

Returns a Boolean value that indicates whether the user can modify the specified persistent store.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func canModifyManagedObjects(in store: NSPersistentStore) -> Bool
```

## Parameters 

`store`  

The persistent store.

## Return Value

true if the user can modify records in the persistent store’s CloudKit database; otherwise, false.

## Discussion

Use this method to determine whether the user is able to write any records to the CloudKit database. To find out if the user can modify a specific object, use the canUpdateRecord(forManagedObjectWith:) and canDeleteRecord(forManagedObjectWith:) methods instead.

This method always returns true for persistent stores that manage the user’s private CloudKit database.

## See Also

### Checking Permissions

func canUpdateRecord(forManagedObjectWith: NSManagedObjectID) -> Bool

Returns a Boolean value that indicates whether the user can modify the managed object’s underlying CloudKit record.

func canDeleteRecord(forManagedObjectWith: NSManagedObjectID) -> Bool

Returns a Boolean value that indicates whether the user can delete the managed object’s underlying CloudKit record.

