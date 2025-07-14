

- Assignables
- AssignableDocument
- AssignableDocument.Page
-  AssignableDocument.Page.ID 

Structure

# AssignableDocument.Page.ID

A type representing the stable identity of this page.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct ID
```

## Topics

### Creating a page identifier

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

typealias Element

The document element type that this reference is for.

### Operators

static func == (AssignableDocument.Page.ID, AssignableDocument.Page.ID) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var debugDescription: String

A textual representation of this instance, suitable for debugging.

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

- CustomDebugStringConvertible
- Decodable
- DocumentElementID
- Encodable
- Equatable
- Hashable

## See Also

### Inspecting a page

var id: AssignableDocument.Page.ID

The stable identity of this page.

var size: CGSize

The dimensions of the page in this document.

typealias Document

The document type this element is for.

