

- CloudKit JS
- CloudKit.Container
-  getDatabaseWithDatabaseScope 

Instance Method

# getDatabaseWithDatabaseScope

Returns the specified (public, private, or shared) database.

CloudKit JS 1.0+

``` source
CloudKit.Database getDatabaseWithDatabaseScope(
 CloudKit.DatabaseScope databaseScope
);
```

## Parameters 

`databaseScope`  

Specifies the type of database to return.

## Return Value

The specified database.

## Discussion

This is a convenience method that you can use instead of the specific properties.

## See Also

### Getting the Public and Private Databases

publicCloudDatabase

The database containing the data shared by all users.

privateCloudDatabase

The database containing the user’s private data.

sharedCloudDatabase

The database containing shared records accepted by the current user.

