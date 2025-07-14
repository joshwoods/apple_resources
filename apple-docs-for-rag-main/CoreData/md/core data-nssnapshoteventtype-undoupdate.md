

- Core Data
- NSSnapshotEventType
-  undoUpdate 

Type Property

# undoUpdate

Specifies a change due to a property-level undo.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var undoUpdate: NSSnapshotEventType { get }
```

## See Also

### Event Types

static var undoInsertion: NSSnapshotEventType

Specifies a change due to undo from insertion.

static var undoDeletion: NSSnapshotEventType

Specifies a change due to undo from deletion.

static var rollback: NSSnapshotEventType

Specifies a change due to the managed object context being rolled back.

static var refresh: NSSnapshotEventType

Specifies a change due to the managed object being refreshed.

static var mergePolicy: NSSnapshotEventType

Specifies a change due to conflict resolution during a save operation.

