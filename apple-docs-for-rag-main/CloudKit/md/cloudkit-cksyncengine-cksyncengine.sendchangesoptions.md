

- CloudKit
- CKSyncEngine
-  CKSyncEngine.SendChangesOptions 

Structure

# CKSyncEngine.SendChangesOptions

A set of options to use with a send operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct SendChangesOptions
```

## Topics

### Managing attributes

var operationGroup: CKOperationGroup

The operation group to use for the underlying CloudKit operations.

### Initializers

init(scope: CKSyncEngine.SendChangesOptions.Scope, operationGroup: CKOperationGroup?)

### Instance Properties

var scope: CKSyncEngine.SendChangesOptions.Scope

### Enumerations

enum Scope

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Invoking manual sync operations

func fetchChanges(CKSyncEngine.FetchChangesOptions) async throws

Fetches pending remote changes from the server.

struct FetchChangesOptions

A set of options to use with a fetch operation.

func sendChanges(CKSyncEngine.SendChangesOptions) async throws

Sends pending local changes to the server.

