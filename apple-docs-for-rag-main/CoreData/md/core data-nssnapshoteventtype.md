

- Core Data
-  NSSnapshotEventType 

Structure

# NSSnapshotEventType

Constants that specify the reason the managed object may need to reinitialize its values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct NSSnapshotEventType
```

## Topics

### Event Types

static var undoInsertion: NSSnapshotEventType

Specifies a change due to undo from insertion.

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

### Initializers

init(rawValue: UInt)

Creates a snapshot event using a raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

