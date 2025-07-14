

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
- CKSyncEngine.Event.FetchedDatabaseChanges
-  modifications 

Instance Property

# modifications

The fetched record modifications.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
let modifications: [CKDatabase.DatabaseChange.Modification]
```

## See Also

### Accessing changes

let deletions: [CKDatabase.DatabaseChange.Deletion]

The fetched record deletions.

enum CKSyncEngineZoneDeletionReason

Describes the reason for a record zone deletion.

