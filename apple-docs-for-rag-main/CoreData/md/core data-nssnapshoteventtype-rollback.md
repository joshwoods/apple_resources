

- Core Data
- NSSnapshotEventType
-  rollback 

Type Property

# rollback

Specifies a change due to the managed object context being rolled back.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var rollback: NSSnapshotEventType { get }
```

## See Also

### Event Types

static var undoInsertion: NSSnapshotEventType

Specifies a change due to undo from insertion.

static var undoDeletion: NSSnapshotEventType

Specifies a change due to undo from deletion.

static var undoUpdate: NSSnapshotEventType

Specifies a change due to a property-level undo.

static var refresh: NSSnapshotEventType

Specifies a change due to the managed object being refreshed.

static var mergePolicy: NSSnapshotEventType

Specifies a change due to conflict resolution during a save operation.

