

- Assignables
- AssignedWorkDocument
- AssignedWorkDocument.Page
-  AssignedWorkDocument.Page.ID 

Structure

# AssignedWorkDocument.Page.ID

A type representing the stable identity of this page.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct ID
```

## Topics

### Creating a page identifier

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Getting the page identifier

var assignableDocumentPageID: AssignableDocument.Page.ID

The AssignableDocument page ID that this work page ID corresponds to.

typealias Element

The document element type that this reference is for.

### Operators

static func == (AssignedWorkDocument.Page.ID, AssignedWorkDocument.Page.ID) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- DocumentElementID
- Encodable
- Equatable
- Hashable

## See Also

### Inspecting the properties

var assignableDocumentPageID: AssignableDocument.Page.ID

The AssignableDocument page ID that this work page ID corresponds to.

var id: AssignedWorkDocument.Page.ID

The stable identity of this page.

typealias Document

The document type this element is for.

typealias Document

The document type this element is for.

