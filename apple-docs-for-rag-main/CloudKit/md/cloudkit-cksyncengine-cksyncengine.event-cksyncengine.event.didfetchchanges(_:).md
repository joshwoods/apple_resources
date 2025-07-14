

- CloudKit
- CKSyncEngine
- CKSyncEngine.Event
-  CKSyncEngine.Event.didFetchChanges(\_:) 

Case

# CKSyncEngine.Event.didFetchChanges(\_:)

An event that indicates the database fetch is done.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case didFetchChanges(CKSyncEngine.Event.DidFetchChanges)
```

## See Also

### Remote database changes

case willFetchChanges(CKSyncEngine.Event.WillFetchChanges)

An event indicating an imminent database fetch.

struct WillFetchChanges

A type that provides information about an imminent database fetch.

case fetchedDatabaseChanges(CKSyncEngine.Event.FetchedDatabaseChanges)

An event indicating there are fetched database changes to process.

struct FetchedDatabaseChanges

A type that provides information about fetched database changes.

struct DidFetchChanges

A type that provides information about a finished database fetch.

