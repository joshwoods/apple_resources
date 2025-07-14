

- Core Data
- NSSnapshotEventType
-  undoInsertion 

Type Property

# undoInsertion

Specifies a change due to undo from insertion.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var undoInsertion: NSSnapshotEventType { get }
```

## See Also

### Event Types

static var undoDeletion: NSSnapshotEventType

Specifies a change due to undo from deletion.

static var undoUpdate: NSSnapshotEventType

Specifies a change due to a property-level undo.

static var rollback: NSSnapshotEventType

Specifies a change due to the managed object context being rolled back.

static var refresh: NSSnapshotEventType

Specifies a change due to the managed object being refreshed.

static var mergePolicy: NSSnapshotEventType

Specifies a change due to conflict resolution during a save operation.

