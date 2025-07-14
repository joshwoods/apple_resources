

- CloudKit JS
- CloudKit.Container
-  sharedCloudDatabase 

Instance Property

# sharedCloudDatabase

The database containing shared records accepted by the current user.

CloudKit JS 1.0+

``` source
readonly attribute CloudKit.Database sharedCloudDatabase;
```

## Discussion

The shared database allows the current user (a participant) to access records shared by other users (owners). Shared records are stored in the owner’s container and count towards the owner’s iCloud account storage quota.

## See Also

### Getting the Public and Private Databases

publicCloudDatabase

The database containing the data shared by all users.

privateCloudDatabase

The database containing the user’s private data.

getDatabaseWithDatabaseScope

Returns the specified (public, private, or shared) database.

