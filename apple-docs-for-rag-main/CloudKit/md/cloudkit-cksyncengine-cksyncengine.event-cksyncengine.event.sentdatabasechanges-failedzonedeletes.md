

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.SentDatabaseChanges
-  failedZoneDeletes 

Instance Property

# failedZoneDeletes

The unique identifiers of the record zones CloudKit is unable to delete, and the reasons why.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
let failedZoneDeletes: [CKRecordZone.ID : CKError]
```

## See Also

### Accessing failed changes

let failedZoneSaves: [CKSyncEngine.Event.SentDatabaseChanges.FailedZoneSave]

The record zones that CloudKit is unable to modify.

struct FailedZoneSave

A type that describes an unsuccessful attempt to modify a single record zone.

