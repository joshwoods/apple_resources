

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.WillFetchRecordZoneChanges 

Structure

# CKSyncEngine.Event.WillFetchRecordZoneChanges

A type that provides information about an imminent fetch of changes in a record zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct WillFetchRecordZoneChanges
```

## Topics

### Identifying the record zone

let zoneID: CKRecordZone.ID

The associated record zone’s unique identifier.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Remote record zone changes

case willFetchRecordZoneChanges(CKSyncEngine.Event.WillFetchRecordZoneChanges)

An event indicating an imminent fetch of changes in a record zone.

case fetchedRecordZoneChanges(CKSyncEngine.Event.FetchedRecordZoneChanges)

An event indicating there are fetched record zone changes to process.

struct FetchedRecordZoneChanges

A type that provides information about fetched record zone changes.

case didFetchRecordZoneChanges(CKSyncEngine.Event.DidFetchRecordZoneChanges)

An event that indicates the record zone fetch is done.

struct DidFetchRecordZoneChanges

A type that provides information about a finished record zone fetch.

