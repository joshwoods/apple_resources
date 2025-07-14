

- CloudKit
- CKShare
-  init(rootRecord:) 

Initializer

# init(rootRecord:)

Creates a new share for the specified record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(rootRecord: CKRecord)
```

## Parameters 

`rootRecord`  

The record to share.

## Discussion

When saving a newly created CKShare, you must save the share and its rootRecord in the same CKModifyRecordsOperation batch.

## See Also

### Creating a Share

init(coder: NSCoder)

Creates a share from a serialized instance.

init(rootRecord: CKRecord, shareID: CKRecord.ID)

Creates a new share for the specified record and record ID.

init(recordZoneID: CKRecordZone.ID)

Creates a new share for the specified record zone.

