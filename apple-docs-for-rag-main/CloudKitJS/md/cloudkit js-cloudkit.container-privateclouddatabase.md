

- CloudKit JS
- CloudKit.Container
-  privateCloudDatabase 

Instance Property

# privateCloudDatabase

The database containing the user’s private data.

CloudKit JS 1.0+

``` source
readonly attribute CloudKit.Database privateCloudDatabase;
```

## See Also

### Getting the Public and Private Databases

publicCloudDatabase

The database containing the data shared by all users.

sharedCloudDatabase

The database containing shared records accepted by the current user.

getDatabaseWithDatabaseScope

Returns the specified (public, private, or shared) database.

