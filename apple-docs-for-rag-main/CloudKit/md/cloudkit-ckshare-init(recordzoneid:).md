

- CloudKit
- CKShare
-  init(recordZoneID:) 

Initializer

# init(recordZoneID:)

Creates a new share for the specified record zone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(recordZoneID: CKRecordZone.ID)
```

## Parameters 

`recordZoneID`  

The ID of the record zone to share.

## Discussion

A shared record zone must have the zoneWideSharing capability. Custom record zones that you create in the user’s private database have this capability by default. A record zone, and the records it contains, can take part in only a single share.

After accepting a share invite, CloudKit adds the records of the shared record zone to a new zone in the participant’s shared database. Use CKFetchDatabaseChangesOperation to fetch the ID of the new record zone. Then configure CKFetchRecordZoneChangesOperation with that record zone ID and execute the operation to fetch the records.

If you use CKFetchShareMetadataOperation to fetch the metadata for a shared record zone, the operation ignores the shouldFetchRootRecord and rootRecordDesiredKeys properties because, unlike a shared record hierarchy, a record zone doesn’t have a nominated root record.

## See Also

### Creating a Share

init(coder: NSCoder)

Creates a share from a serialized instance.

convenience init(rootRecord: CKRecord)

Creates a new share for the specified record.

init(rootRecord: CKRecord, shareID: CKRecord.ID)

Creates a new share for the specified record and record ID.

