

- CloudKit
- CKSyncEngineSyncReason
-  CKSyncEngineSyncReason.manual 

Case

# CKSyncEngineSyncReason.manual

A manual sync operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case manual
```

## Discussion

The sync engine uses this reason only when your app invokes the fetchChangesWithCompletionHandler: and sendChangesWithCompletionHandler: methods and their variants.

## See Also

### Sync reasons

case scheduled

A scheduled sync operation.

