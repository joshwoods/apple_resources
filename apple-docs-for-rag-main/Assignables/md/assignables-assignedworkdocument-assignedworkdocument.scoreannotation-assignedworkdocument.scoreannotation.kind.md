

- Assignables
- AssignedWorkDocument
- AssignedWorkDocument.ScoreAnnotation
-  AssignedWorkDocument.ScoreAnnotation.Kind 

Enumeration

# AssignedWorkDocument.ScoreAnnotation.Kind

The kind of a score annotation.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum Kind
```

## Topics

### Score annotations

case bonus

A score mark indicating a bonus to an answer.

case correct

A score mark indicating an correct answer.

case incorrect

A score mark indicating an incorrect answer.

case unknown

An unknown kind. This value may occur if an older version of this framework is deserializing a newer document version.

### Creating a score annotation

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [AssignedWorkDocument.ScoreAnnotation.Kind]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- RawRepresentable

## See Also

### Inspecting a score annotation

typealias ID

A type representing the stable identity of this score annotation.

var id: AssignedWorkDocument.ScoreAnnotation.ID

The stable identity of this score annotation.

var kind: AssignedWorkDocument.ScoreAnnotation.Kind

The kind of score annotation this is. e.g. Incorrect or correct mark.

var location: CGPoint

The location of the score annotation on the associated page.

var pageID: AssignedWorkDocument.Page.ID?

The ID of the page this score annotation is for.

typealias Document

The document type this element is for.

