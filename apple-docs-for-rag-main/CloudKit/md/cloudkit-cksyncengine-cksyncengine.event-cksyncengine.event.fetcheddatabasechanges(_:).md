

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.fetchedDatabaseChanges(\_:) 

Case

# CKSyncEngine.Event.fetchedDatabaseChanges(\_:)

An event indicating there are fetched database changes to process.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case fetchedDatabaseChanges(CKSyncEngine.Event.FetchedDatabaseChanges)
```

## See Also

### Remote database changes

case willFetchChanges(CKSyncEngine.Event.WillFetchChanges)

An event indicating an imminent database fetch.

struct WillFetchChanges

A type that provides information about an imminent database fetch.

struct FetchedDatabaseChanges

A type that provides information about fetched database changes.

case didFetchChanges(CKSyncEngine.Event.DidFetchChanges)

An event that indicates the database fetch is done.

struct DidFetchChanges

A type that provides information about a finished database fetch.

