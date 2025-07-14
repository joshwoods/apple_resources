

- CloudKit
- CKSyncEngineDelegate
-  nextFetchChangesOptions(\_:syncEngine:) 

Instance Method

# nextFetchChangesOptions(\_:syncEngine:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func nextFetchChangesOptions(
    _ context: CKSyncEngine.FetchChangesContext,
    syncEngine: CKSyncEngine
) async -> CKSyncEngine.FetchChangesOptions
```

**Required** Default implementation provided.

## Default Implementations

### CKSyncEngineDelegate Implementations

func nextFetchChangesOptions(CKSyncEngine.FetchChangesContext, syncEngine: CKSyncEngine) async -> CKSyncEngine.FetchChangesOptions

