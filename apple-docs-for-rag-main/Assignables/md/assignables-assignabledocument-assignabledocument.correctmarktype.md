

- Assignables
- AssignableDocument
-  AssignableDocument.CorrectMarkType 

Enumeration

# AssignableDocument.CorrectMarkType

The glyph to use that represents a correct mark.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum CorrectMarkType
```

## Topics

### Mark types

case checkmark

Correct marks are shown with checkmarks.

case numeric

Correct marks are shown with numbers.

case star

Correct marks are shown with stars.

case unknown

Unknown

### Inspecting a type

var debugDescription: String

A textual representation of this instance, suitable for debugging.

var id: AssignableDocument.CorrectMarkType

The stable identity of this enum value.

### Operators

static func == (AssignableDocument.CorrectMarkType, AssignableDocument.CorrectMarkType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Type Properties

static var allCases: [AssignableDocument.CorrectMarkType]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Identifiable

## See Also

### Getting the configuration

typealias Configuration

The configuration for an assessment which contains options for display of marks and their point values.

var configuration: some AssignableDocumentConfiguration

The configuration of this assessment which contains options for display of marks and their point values.

