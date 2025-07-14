

- Assignables
- AssignedWorkDocument
-  AssignedWorkDocument.ScoreAnnotation 

Structure

# AssignedWorkDocument.ScoreAnnotation

A score mark on page of the work document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct ScoreAnnotation
```

## Topics

### Creating a score annotation

init(id: AssignedWorkDocument.ScoreAnnotation.ID, pageID: AssignedWorkDocument.Page.ID?, location: CGPoint, kind: AssignedWorkDocument.ScoreAnnotation.Kind)

Initializes an instance of this object with the given values.

### Inspecting a score annotation

typealias ID

A type representing the stable identity of this score annotation.

var id: AssignedWorkDocument.ScoreAnnotation.ID

The stable identity of this score annotation.

enum Kind

The kind of a score annotation.

var kind: AssignedWorkDocument.ScoreAnnotation.Kind

The kind of score annotation this is. e.g. Incorrect or correct mark.

var location: CGPoint

The location of the score annotation on the associated page.

var pageID: AssignedWorkDocument.Page.ID?

The ID of the page this score annotation is for.

typealias Document

The document type this element is for.

### Comparing score annotations

static func == (AssignedWorkDocument.ScoreAnnotation, AssignedWorkDocument.ScoreAnnotation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Hashing the score annotation

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Instance Properties

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- AssignedWorkDocumentElement
- Copyable
- DocumentElement
- Equatable
- Hashable
- Identifiable

## See Also

### Computing the score

func computeScore() -> Double

Gathers all of the points based on all the `AssignedWorkDocument.ScoreAnnotation`s in the document and its `kind` property.

