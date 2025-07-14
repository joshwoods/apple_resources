

- CloudKit
- CKSyncEngine
- CKSyncEngine.SyncReason
-  CKSyncEngine.SyncReason.manual 

Case

# CKSyncEngine.SyncReason.manual

A manual sync operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
case manual
```

## Discussion

The sync engine uses this reason only when your app invokes the fetchChanges(_:) and sendChanges(_:) methods.

## See Also

### Sync reasons

case scheduled

A scheduled sync operation.

