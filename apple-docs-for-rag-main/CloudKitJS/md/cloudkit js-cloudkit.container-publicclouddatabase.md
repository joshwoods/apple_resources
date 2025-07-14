

- CloudKit JS
- CloudKit.Container
-  publicCloudDatabase 

Instance Property

# publicCloudDatabase

The database containing the data shared by all users.

CloudKit JS 1.0+

``` source
readonly attribute CloudKit.Database publicCloudDatabase;
```

## See Also

### Getting the Public and Private Databases

privateCloudDatabase

The database containing the user’s private data.

sharedCloudDatabase

The database containing shared records accepted by the current user.

getDatabaseWithDatabaseScope

Returns the specified (public, private, or shared) database.

