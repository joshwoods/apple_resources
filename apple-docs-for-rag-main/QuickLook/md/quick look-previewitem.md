

- Quick Look
-  PreviewItem 

Structure

# PreviewItem

An item to preview in the preview application.

visionOS 2.0+

``` source
struct PreviewItem
```

## Topics

### Operators

static func == (PreviewItem, PreviewItem) -> Bool

Returns a Boolean value that indicates whether two preview items are equal.

### Initializers

init(url: URL, displayName: String?, editingMode: EditingMode)

Create a preview item from a URL and, optionally, a displayName and editingMode.

### Instance Properties

let displayName: String?

An optional display name to present for the preview item.

let editingMode: EditingMode

The editingMode for the preview item.

let id: UUID

The stable identity of the preview item.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

## Relationships

### Conforms To

- Equatable
- Hashable
- Identifiable
- Sendable

