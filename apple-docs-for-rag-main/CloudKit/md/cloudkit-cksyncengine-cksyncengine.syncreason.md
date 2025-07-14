

- CloudKit
- CKSyncEngine
-  CKSyncEngine.SyncReason 

Enumeration

# CKSyncEngine.SyncReason

Describes the reason for a sync operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
enum SyncReason
```

## Topics

### Sync reasons

case scheduled

A scheduled sync operation.

case manual

A manual sync operation.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Accessing specific attributes

let reason: CKSyncEngine.SyncReason

The reason for the send operation.

enum CKSyncEngineSyncReason

Describes the reason for a sync operation.

let options: CKSyncEngine.SendChangesOptions

The additional options for the send operation.

struct SendChangesOptions

A set of options to use with a send operation.

