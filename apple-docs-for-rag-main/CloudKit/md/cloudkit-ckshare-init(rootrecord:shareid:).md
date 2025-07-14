

- CloudKit
- CKShare
-  init(rootRecord:shareID:) 

Initializer

# init(rootRecord:shareID:)

Creates a new share for the specified record and record ID.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    rootRecord: CKRecord,
    shareID: CKRecord.ID
)
```

## Parameters 

`rootRecord`  

The record to share.

`shareID`  

The CKRecord.ID for the share.

## Discussion

When saving a newly created CKShare, save the share and its rootRecord in the same CKModifyRecordsOperation batch.

## See Also

### Creating a Share

init(coder: NSCoder)

Creates a share from a serialized instance.

convenience init(rootRecord: CKRecord)

Creates a new share for the specified record.

init(recordZoneID: CKRecordZone.ID)

Creates a new share for the specified record zone.

