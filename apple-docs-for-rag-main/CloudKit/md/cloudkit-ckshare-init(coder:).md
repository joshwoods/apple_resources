

- CloudKit
- CKShare
-  init(coder:) 

Initializer

# init(coder:)

Creates a share from a serialized instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

The coder to use when deserializing the share.

## Discussion

When saving a newly created CKShare, you must save the share and its rootRecord in the same CKModifyRecordsOperation batch.

## See Also

### Creating a Share

convenience init(rootRecord: CKRecord)

Creates a new share for the specified record.

init(rootRecord: CKRecord, shareID: CKRecord.ID)

Creates a new share for the specified record and record ID.

init(recordZoneID: CKRecordZone.ID)

Creates a new share for the specified record zone.

