

- CloudKit
- CKRecordZone
-  init(zoneName:) 

Initializer

# init(zoneName:)

Creates a record zone object with the specified zone name.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
init(zoneName: String)
```

## Parameters 

`zoneName`  

The name of the new zone. Zone names inside a user’s private database are unique, consist of up to 255 ASCII characters, and don’t start with an underscore. One way to ensure the uniqueness of zone names is to create a string from a UUID, but you can also use other techniques.

If this parameter is `nil` or is an empty string, the method throws an exception.

## Return Value

The new custom zone, or `nil` if CloudKit can’t create the zone.

## Discussion

Use this method to create a new record zone. The new zone has the name you provide and the zone’s owner is the current user. After creating the zone, save it to the server using a CKModifyRecordZonesOperation object or the save(_:completionHandler:) method of CKDatabase. You must save the zone to the server before you attempt to save any records to that zone.

Don’t use this method to create a `CKRecordZone` object that corresponds to a zone that already exists in the database. If the zone exists, fetch it using a CKFetchRecordZonesOperation object or the fetch(withRecordZoneID:completionHandler:) method of CKDatabase.

## See Also

### Creating a Record Zone

init(zoneID: CKRecordZone.ID)

Creates a record zone object with the specified zone ID.

class ID

An object that uniquely identifies a record zone in a database.

