

- Core Services
- Search Kit
-  SKIndexType 

Structure

# SKIndexType

Specifies the category of an index.

Mac Catalyst 13.0+macOS 10.3+

``` source
struct SKIndexType
```

## Topics

### Constants

var kSKIndexUnknown: SKIndexType

Specifies an unknown index type.

var kSKIndexInverted: SKIndexType

Specifies an inverted index, mapping terms to documents.

var kSKIndexVector: SKIndexType

Specifies a vector index, mapping documents to terms.

var kSKIndexInvertedVector: SKIndexType

Specifies an index type with all the capabilities of an inverted and a vector index.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- Hashable
- RawRepresentable

