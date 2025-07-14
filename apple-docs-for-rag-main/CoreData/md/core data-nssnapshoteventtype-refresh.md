

- Core Data
- NSSnapshotEventType
-  refresh 

Type Property

# refresh

Specifies a change due to the managed object being refreshed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var refresh: NSSnapshotEventType { get }
```

## See Also

### Event Types

static var undoInsertion: NSSnapshotEventType

Specifies a change due to undo from insertion.

static var undoDeletion: NSSnapshotEventType

Specifies a change due to undo from deletion.

static var undoUpdate: NSSnapshotEventType

Specifies a change due to a property-level undo.

static var rollback: NSSnapshotEventType

Specifies a change due to the managed object context being rolled back.

static var mergePolicy: NSSnapshotEventType

Specifies a change due to conflict resolution during a save operation.

