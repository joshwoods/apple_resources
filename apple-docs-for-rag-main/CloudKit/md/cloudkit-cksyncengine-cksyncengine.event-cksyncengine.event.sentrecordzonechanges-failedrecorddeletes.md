

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.SentRecordZoneChanges
-  failedRecordDeletes 

Instance Property

# failedRecordDeletes

The unique identifiers of the records CloudKit is unable to delete, and the reasons why.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
let failedRecordDeletes: [CKRecord.ID : CKError]
```

## See Also

### Accessing failed changes

let failedRecordSaves: [CKSyncEngine.Event.SentRecordZoneChanges.FailedRecordSave]

The records that CloudKit is unable to modify.

struct FailedRecordSave

A type that describes an unsuccessful attempt to modify a single record.

