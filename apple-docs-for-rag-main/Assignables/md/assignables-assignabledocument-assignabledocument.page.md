

- Assignables
- AssignableDocument
-  AssignableDocument.Page 

Structure

# AssignableDocument.Page

A page within this assignable document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct Page
```

## Topics

### Inspecting a page

struct ID

A type representing the stable identity of this page.

var id: AssignableDocument.Page.ID

The stable identity of this page.

var size: CGSize

The dimensions of the page in this document.

typealias Document

The document type this element is for.

### Comparing pages

static func == (AssignableDocument.Page, AssignableDocument.Page) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Hashing a page

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Instance Properties

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var hashValue: Int

The hash value.

var rotation: Measurement&lt;UnitAngle>

The rotation of the page in this document.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- AssignableDocumentElement
- CustomDebugStringConvertible
- DocumentElement
- Equatable
- Hashable
- Identifiable
- MergeableDocumentPage

