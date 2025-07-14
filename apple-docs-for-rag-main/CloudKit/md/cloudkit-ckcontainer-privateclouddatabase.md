

- CloudKit
- CKContainer
-  privateCloudDatabase 

Instance Property

# privateCloudDatabase

The user’s private database.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var privateCloudDatabase: CKDatabase { get }
```

## Discussion

The user’s private database is only available if the device has an iCloud account. Only the user can access their private database, by default. They own all of the database’s content and can view and modify that content. Data in the private database isn’t visible in the developer portal.

Data in the private database counts toward the user’s iCloud storage quota.

If there isn’t an iCloud account on the user’s device, this property still returns a database, but any attempt to use it results in an error. To determine if there is an iCloud account on the device, use the accountStatus(completionHandler:) method.

## See Also

### Getting the Public and Private Databases

var publicCloudDatabase: CKDatabase

The app’s public database.

var sharedCloudDatabase: CKDatabase

The database that contains shared data.

func database(with: CKDatabase.Scope) -> CKDatabase

Returns the database with the specified scope.

