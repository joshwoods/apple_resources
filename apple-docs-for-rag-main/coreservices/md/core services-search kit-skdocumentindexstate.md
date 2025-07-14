

- Core Services
- Search Kit
-  SKDocumentIndexState 

Structure

# SKDocumentIndexState

The indexing state of a document.

Mac Catalyst 13.0+macOS 10.3+

``` source
struct SKDocumentIndexState
```

## Topics

### Constants

var kSKDocumentStateNotIndexed: SKDocumentIndexState

Specifies that the document is not indexed.

var kSKDocumentStateIndexed: SKDocumentIndexState

Specifies that the document is indexed.

var kSKDocumentStateAddPending: SKDocumentIndexState

Specifies that the document is not in the index but will be added after the index is flushed or closed.

var kSKDocumentStateDeletePending: SKDocumentIndexState

Specifies that the document is in the index but will be deleted after the index is flushed or closed.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- Hashable
- RawRepresentable

