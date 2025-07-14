

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.didFetchRecordZoneChanges(\_:) 

Case

# CKSyncEngine.Event.didFetchRecordZoneChanges(\_:)

An event that indicates the record zone fetch is done.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case didFetchRecordZoneChanges(CKSyncEngine.Event.DidFetchRecordZoneChanges)
```

## See Also

### Remote record zone changes

case willFetchRecordZoneChanges(CKSyncEngine.Event.WillFetchRecordZoneChanges)

An event indicating an imminent fetch of changes in a record zone.

struct WillFetchRecordZoneChanges

A type that provides information about an imminent fetch of changes in a record zone.

case fetchedRecordZoneChanges(CKSyncEngine.Event.FetchedRecordZoneChanges)

An event indicating there are fetched record zone changes to process.

struct FetchedRecordZoneChanges

A type that provides information about fetched record zone changes.

struct DidFetchRecordZoneChanges

A type that provides information about a finished record zone fetch.

