

- CloudKit
- CKRecordZone
-  init(zoneID:) 

Initializer

# init(zoneID:)

Creates a record zone object with the specified zone ID.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
init(zoneID: CKRecordZone.ID)
```

## Parameters 

`zoneID`  

The ID for the new zone. This parameter must not be `nil`.

## Return Value

The custom record zone, or `nil` if CloudKit can’t create the zone.

## Discussion

Use this method when you want to create a new record zone from the information in a zone ID. After creating the zone, save it to the server using a CKModifyRecordZonesOperation object or the save(_:completionHandler:) method of CKDatabase.

Don’t use this method to create a CKRecordZone object that corresponds to a zone that already exists in the database. If the zone exists, fetch it using a CKFetchRecordZonesOperation object or the fetch(withRecordZoneID:completionHandler:) method of CKDatabase.

## See Also

### Creating a Record Zone

init(zoneName: String)

Creates a record zone object with the specified zone name.

class ID

An object that uniquely identifies a record zone in a database.

