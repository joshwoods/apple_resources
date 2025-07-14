

- SwiftData
- DataStore
-  invalidateState(for:) 

Instance Method

# invalidateState(for:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
func invalidateState(for editingState: EditingState)
```

**Required** Default implementation provided.

## Default Implementations

### DataStore Implementations

func invalidateState(for: EditingState)

## See Also

### Sharing cached data between model contexts

func initializeState(for: EditingState)

**Required** Default implementation provided.

struct EditingState

func cachedSnapshots(for: [PersistentIdentifier], editingState: EditingState) throws -> [PersistentIdentifier : Self.Snapshot]

**Required** Default implementation provided.

