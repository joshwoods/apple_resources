

- SwiftData
-  EditingState 

Structure

# EditingState

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct EditingState
```

## Topics

### Instance Properties

var author: String?

let id: UUID

The stable identity of the entity associated with this instance.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Sharing cached data between model contexts

func initializeState(for: EditingState)

**Required** Default implementation provided.

func cachedSnapshots(for: [PersistentIdentifier], editingState: EditingState) throws -> [PersistentIdentifier : Self.Snapshot]

**Required** Default implementation provided.

func invalidateState(for: EditingState)

**Required** Default implementation provided.

