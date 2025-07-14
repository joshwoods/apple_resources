

- CloudKit
- CKContainer
-  publicCloudDatabase 

Instance Property

# publicCloudDatabase

The app’s public database.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var publicCloudDatabase: CKDatabase { get }
```

## Discussion

This database is available regardless of whether the user’s device has an iCloud account. The contents of the public database are readable by all users of the app, and users have write access to the records, and other objects, they create. The public database’s contents are visible in the developer portal, where you can assign roles to users and restrict access as necessary.

Data in the public database counts toward your app’s iCloud storage quota.

## See Also

### Getting the Public and Private Databases

var privateCloudDatabase: CKDatabase

The user’s private database.

var sharedCloudDatabase: CKDatabase

The database that contains shared data.

func database(with: CKDatabase.Scope) -> CKDatabase

Returns the database with the specified scope.

