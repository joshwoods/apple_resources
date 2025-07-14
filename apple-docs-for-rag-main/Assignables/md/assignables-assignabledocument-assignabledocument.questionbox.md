

- Assignables
- AssignableDocument
-  AssignableDocument.QuestionBox 

Structure

# AssignableDocument.QuestionBox

A box on a page for a question.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct QuestionBox
```

### Creating a question box

- init(id:pageID:bounds:)

### Inspecting the question box

- bounds

- AssignableDocument.QuestionBox.ID

- id

- pageID

- AssignableDocument.QuestionBox.Document

### Comparing question boxes

- \`\`==(*:*:)\`

### Hashing the question box

- hash(into:)

## Topics

### Operators

static func == (AssignableDocument.QuestionBox, AssignableDocument.QuestionBox) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(id: AssignableDocument.QuestionBox.ID, pageID: AssignableDocument.Page.ID, bounds: CGRect)

Initialize a question box.

### Instance Properties

var bounds: CGRect

The bounds of the question box on the page.

var hashValue: Int

The hash value.

var id: AssignableDocument.QuestionBox.ID

The stable identity of this box.

var pageID: AssignableDocument.Page.ID?

A read-only property providing the identifier of the page that owns this question box. If the box is not yet assigned to a page, this value is `nil`.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias Document

The document type this element is for.

typealias ID

A type representing the stable identity of this box.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- AssignableDocumentElement
- DocumentElement
- Equatable
- Hashable
- Identifiable

## See Also

### Inspecting an assignable document

typealias ID

A type representing the stable identity of this document.

var id: AssignableDocument.ID

The stable identity of this document.

var isMultiPageDocument: Bool

`true`, if this document has more than one page; `false`, otherwise.

var isPartial: Bool

Denotes whether or not this document is a partial one.

enum PartIDs

An enumeration containing the identities of parts managed by this view.

var partIDs: [AssignableDocument.PartID]

Returns a collection of identifiers reflecting the manifest of parts available in the document.

struct Question

A question in the assignable document.

var questions: [AssignableDocument.Question]

A collection of questions defined for this assignable.

typealias Element

The type for elements of this document. An element is a component of the document such as a page or question.

enum Error

Errors for this document type.

