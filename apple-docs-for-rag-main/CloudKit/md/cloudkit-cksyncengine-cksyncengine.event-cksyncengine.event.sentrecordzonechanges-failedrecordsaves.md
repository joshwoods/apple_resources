

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.SentRecordZoneChanges
-  failedRecordSaves 

Instance Property

# failedRecordSaves

The records that CloudKit is unable to modify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
let failedRecordSaves: [CKSyncEngine.Event.SentRecordZoneChanges.FailedRecordSave]
```

## See Also

### Accessing failed changes

let failedRecordDeletes: [CKRecord.ID : CKError]

The unique identifiers of the records CloudKit is unable to delete, and the reasons why.

struct FailedRecordSave

A type that describes an unsuccessful attempt to modify a single record.

