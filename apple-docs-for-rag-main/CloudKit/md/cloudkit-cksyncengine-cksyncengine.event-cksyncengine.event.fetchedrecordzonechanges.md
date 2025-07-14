

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.FetchedRecordZoneChanges 

Structure

# CKSyncEngine.Event.FetchedRecordZoneChanges

A type that provides information about fetched record zone changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct FetchedRecordZoneChanges
```

## Overview

Note

Although CloudKit doesn’t guarantee the order of fetched record zone changes, the typical order for both deletions and modifications is oldest to newest.

## Topics

### Accessing changes

let deletions: [CKDatabase.RecordZoneChange.Deletion]

The fetched record zone deletions.

let modifications: [CKDatabase.RecordZoneChange.Modification]

The fetched record zone modifications.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Remote record zone changes

case willFetchRecordZoneChanges(CKSyncEngine.Event.WillFetchRecordZoneChanges)

An event indicating an imminent fetch of changes in a record zone.

struct WillFetchRecordZoneChanges

A type that provides information about an imminent fetch of changes in a record zone.

case fetchedRecordZoneChanges(CKSyncEngine.Event.FetchedRecordZoneChanges)

An event indicating there are fetched record zone changes to process.

case didFetchRecordZoneChanges(CKSyncEngine.Event.DidFetchRecordZoneChanges)

An event that indicates the record zone fetch is done.

struct DidFetchRecordZoneChanges

A type that provides information about a finished record zone fetch.

