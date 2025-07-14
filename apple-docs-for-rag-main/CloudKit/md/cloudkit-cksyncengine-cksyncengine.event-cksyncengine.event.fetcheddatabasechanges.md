

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.FetchedDatabaseChanges 

Structure

# CKSyncEngine.Event.FetchedDatabaseChanges

A type that provides information about fetched database changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct FetchedDatabaseChanges
```

## Overview

Note

Although CloudKit doesn’t guarantee the order of fetched database changes, the typical order for both deletions and modifications is oldest to newest.

## Topics

### Accessing changes

let deletions: [CKDatabase.DatabaseChange.Deletion]

The fetched record deletions.

enum CKSyncEngineZoneDeletionReason

Describes the reason for a record zone deletion.

let modifications: [CKDatabase.DatabaseChange.Modification]

The fetched record modifications.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Remote database changes

case willFetchChanges(CKSyncEngine.Event.WillFetchChanges)

An event indicating an imminent database fetch.

struct WillFetchChanges

A type that provides information about an imminent database fetch.

case fetchedDatabaseChanges(CKSyncEngine.Event.FetchedDatabaseChanges)

An event indicating there are fetched database changes to process.

case didFetchChanges(CKSyncEngine.Event.DidFetchChanges)

An event that indicates the database fetch is done.

struct DidFetchChanges

A type that provides information about a finished database fetch.

