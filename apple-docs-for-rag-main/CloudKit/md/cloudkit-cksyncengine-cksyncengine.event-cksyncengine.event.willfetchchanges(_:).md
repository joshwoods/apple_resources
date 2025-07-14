

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.willFetchChanges(\_:) 

Case

# CKSyncEngine.Event.willFetchChanges(\_:)

An event indicating an imminent database fetch.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case willFetchChanges(CKSyncEngine.Event.WillFetchChanges)
```

## See Also

### Remote database changes

struct WillFetchChanges

A type that provides information about an imminent database fetch.

case fetchedDatabaseChanges(CKSyncEngine.Event.FetchedDatabaseChanges)

An event indicating there are fetched database changes to process.

struct FetchedDatabaseChanges

A type that provides information about fetched database changes.

case didFetchChanges(CKSyncEngine.Event.DidFetchChanges)

An event that indicates the database fetch is done.

struct DidFetchChanges

A type that provides information about a finished database fetch.

