

- Assignables
- AssignedWorkDocument
-  AssignedWorkDocument.Page 

Structure

# AssignedWorkDocument.Page

A page within this assigned work document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct Page
```

## Topics

### Inspecting the properties

var assignableDocumentPageID: AssignableDocument.Page.ID

The AssignableDocument page ID that this work page ID corresponds to.

struct ID

A type representing the stable identity of this page.

var id: AssignedWorkDocument.Page.ID

The stable identity of this page.

typealias Document

The document type this element is for.

typealias Document

The document type this element is for.

### Hashing the page

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing pages

static func == (AssignedWorkDocument.Page, AssignedWorkDocument.Page) -> Bool

Returns a Boolean value indicating whether two values are equal.

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

- AssignedWorkDocumentElement
- Copyable
- CustomDebugStringConvertible
- DocumentElement
- Equatable
- Hashable
- Identifiable
- MergeableDocumentPage

