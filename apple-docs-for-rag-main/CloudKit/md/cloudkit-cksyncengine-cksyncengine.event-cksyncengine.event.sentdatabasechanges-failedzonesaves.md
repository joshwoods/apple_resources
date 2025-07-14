

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.SentDatabaseChanges
-  failedZoneSaves 

Instance Property

# failedZoneSaves

The record zones that CloudKit is unable to modify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
let failedZoneSaves: [CKSyncEngine.Event.SentDatabaseChanges.FailedZoneSave]
```

## See Also

### Accessing failed changes

let failedZoneDeletes: [CKRecordZone.ID : CKError]

The unique identifiers of the record zones CloudKit is unable to delete, and the reasons why.

struct FailedZoneSave

A type that describes an unsuccessful attempt to modify a single record zone.

