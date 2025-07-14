

- Assignables
-  MergeablePartsContainerPartID 

Structure

# MergeablePartsContainerPartID

The ID of a part in a `MergeablePartsContainer`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct MergeablePartsContainerPartID
```

## Topics

### Operators

static func == (MergeablePartsContainerPartID, MergeablePartsContainerPartID) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(String)

Initiailizes an instance of a document part ID.

### Instance Properties

var hashValue: Int

The hash value.

var rawValue: String

The underlying value of the part ID.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Mergeable document

protocol MergeableDocument

Documents conforming to this protocol can merge several copies of the document into a single document.

protocol MergeableDocumentPage

Types conforming to this protocol indicate that they are a page in a MergeableDocument conforming object.

protocol MergeablePartsContainer

Objects conforming to this protocol allow merging in other replicas of themselves or merging in individual parts of themselves.

struct DocumentThumbnail

A structure that contains an image of an entire page or a portion of a page and the ID of the page the image is from.

