

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.willFetchRecordZoneChanges(\_:) 

Case

# CKSyncEngine.Event.willFetchRecordZoneChanges(\_:)

An event indicating an imminent fetch of changes in a record zone.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case willFetchRecordZoneChanges(CKSyncEngine.Event.WillFetchRecordZoneChanges)
```

## See Also

### Remote record zone changes

struct WillFetchRecordZoneChanges

A type that provides information about an imminent fetch of changes in a record zone.

case fetchedRecordZoneChanges(CKSyncEngine.Event.FetchedRecordZoneChanges)

An event indicating there are fetched record zone changes to process.

struct FetchedRecordZoneChanges

A type that provides information about fetched record zone changes.

case didFetchRecordZoneChanges(CKSyncEngine.Event.DidFetchRecordZoneChanges)

An event that indicates the record zone fetch is done.

struct DidFetchRecordZoneChanges

A type that provides information about a finished record zone fetch.

