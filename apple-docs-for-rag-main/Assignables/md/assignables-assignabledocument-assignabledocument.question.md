

- Assignables
- AssignableDocument
-  AssignableDocument.Question 

Structure

# AssignableDocument.Question

A question in the assignable document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct Question
```

## Topics

### Creating a question

init(pageID: AssignableDocument.Page.ID, boxes: [AssignableDocument.QuestionBox], maxScore: Double?)

Initializes an instance of this object with the given values.

### Inspecting a question

var boxes: [AssignableDocument.QuestionBox]

The question boxes on pages that denote question regions. Treated as as set.

typealias ID

A type representing the stable identity of this question.

var id: AssignableDocument.Question.ID

The stable identity of this question.

var maxScore: Double?

An optional manual maximum point value for this question.

struct Thumbnail

The thumbnail type for this question.

typealias Document

The document type this element is for.

### Comparing questions

static func == (AssignableDocument.Question, AssignableDocument.Question) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Hashing a question

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Instance Properties

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- AssignableDocumentElement
- Copyable
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

struct QuestionBox

A box on a page for a question.

var questions: [AssignableDocument.Question]

A collection of questions defined for this assignable.

typealias Element

The type for elements of this document. An element is a component of the document such as a page or question.

enum Error

Errors for this document type.

