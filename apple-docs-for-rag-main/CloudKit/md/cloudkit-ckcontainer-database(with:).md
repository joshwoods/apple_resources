

- CloudKit
- CKContainer
-  database(with:) 

Instance Method

# database(with:)

Returns the database with the specified scope.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func database(with databaseScope: CKDatabase.Scope) -> CKDatabase
```

## Parameters 

`databaseScope`  

The database’s scope. See CKDatabase.Scope for the available options.

## See Also

### Getting the Public and Private Databases

var privateCloudDatabase: CKDatabase

The user’s private database.

var publicCloudDatabase: CKDatabase

The app’s public database.

var sharedCloudDatabase: CKDatabase

The database that contains shared data.

