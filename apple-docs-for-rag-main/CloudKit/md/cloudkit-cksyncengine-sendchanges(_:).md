

- CloudKit
- CKSyncEngine
-  sendChanges(\_:) 

Instance Method

# sendChanges(\_:)

Sends pending local changes to the server.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
final func sendChanges(_ options: CKSyncEngine.SendChangesOptions = .init()) async throws
```

## Parameters 

`options`  

The options to use when sending changes. For more information, see CKSyncEngine.SendChangesOptions.

## Discussion

Use this method to ensure the sync engine sends all pending local changes to the server before your app continues. This isn’t necessary in normal use, as the engine automatically syncs your app’s records. It is useful, however, in scenarios where you require greater control over sync, such as a “Backup now” button or unit tests.

Note

sendChanges(_:) returns only after your sync delegate finishes processing all related send events.

## See Also

### Invoking manual sync operations

func fetchChanges(CKSyncEngine.FetchChangesOptions) async throws

Fetches pending remote changes from the server.

struct FetchChangesOptions

A set of options to use with a fetch operation.

struct SendChangesOptions

A set of options to use with a send operation.

