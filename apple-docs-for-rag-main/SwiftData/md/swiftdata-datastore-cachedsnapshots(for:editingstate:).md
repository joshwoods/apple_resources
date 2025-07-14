

- SwiftData
- DataStore
-  cachedSnapshots(for:editingState:) 

Instance Method

# cachedSnapshots(for:editingState:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
func cachedSnapshots(
    for persistentIdentifiers: [PersistentIdentifier],
    editingState: EditingState
) throws -> [PersistentIdentifier : Self.Snapshot]
```

**Required** Default implementation provided.

## Default Implementations

### DataStore Implementations

func cachedSnapshots(for: [PersistentIdentifier], editingState: EditingState) throws -> [PersistentIdentifier : Self.Snapshot]

## See Also

### Sharing cached data between model contexts

func initializeState(for: EditingState)

**Required** Default implementation provided.

struct EditingState

func invalidateState(for: EditingState)

**Required** Default implementation provided.

