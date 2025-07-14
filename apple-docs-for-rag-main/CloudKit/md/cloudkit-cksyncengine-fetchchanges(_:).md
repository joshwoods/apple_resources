

- CloudKit
- CKSyncEngine
-  fetchChanges(\_:) 

Instance Method

# fetchChanges(\_:)

Fetches pending remote changes from the server.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final func fetchChanges(_ options: CKSyncEngine.FetchChangesOptions = .init()) async throws
```

## Parameters 

`options`  

The options to use when fetching changes. For more information, see CKSyncEngine.FetchChangesOptions.

## Discussion

Use this method to ensure the sync engine immediately fetches all pending remote changes before your app continues. This isn’t necessary in normal use, as the engine automatically syncs your app’s records. It is useful, however, in scenarios where you require more control over sync, such as pull-to-refresh or unit tests.

Note

fetchChanges(_:) returns only after your sync delegate finishes processing all related fetch events.

## See Also

### Invoking manual sync operations

struct FetchChangesOptions

A set of options to use with a fetch operation.

func sendChanges(CKSyncEngine.SendChangesOptions) async throws

Sends pending local changes to the server.

struct SendChangesOptions

A set of options to use with a send operation.

