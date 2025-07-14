

- Assignables
-  BasicDocumentElementID 

Structure

# BasicDocumentElementID

A default implementation for a document element identifier.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct BasicDocumentElementID where Element : DocumentElement
```

## Topics

### Creating an element identifier

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Operators

static func == (BasicDocumentElementID&lt;Element>, BasicDocumentElementID&lt;Element>) -> Bool

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

### Document elements

protocol DocumentElement

Represents an element that is contained within a document. Such elements can have identifiers that uniquely identify them within a document.

protocol DocumentElementID

An identifier for an element in a document.

protocol AssignableDocumentElement

An element of an AssignableDocument.

protocol AssignedWorkDocumentElement

An element of an AssignedWorkDocument.

