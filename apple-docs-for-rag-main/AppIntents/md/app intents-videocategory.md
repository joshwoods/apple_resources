

- App Intents
-  VideoCategory 

Enumeration

# VideoCategory

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+

``` source
enum VideoCategory
```

## Topics

### Enumeration Cases

case freeform

The app supports searching for freeform video content like what may uploaded to social media platforms. This should not be used in cases of highly structured content like movies and episodic tv shows.

case movies

The app supports searching for structured movie content.

case tv

The app supports searching for structured tv content including shows, seasons, or episodes.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var allCases: [VideoCategory]

A collection of all values of this type.

static var caseDisplayRepresentations: [VideoCategory : DisplayRepresentation]

A dictionary that maps each value to the visual elements that represent it.

static var typeDisplayRepresentation: TypeDisplayRepresentation

A short, localized, human-readable name for the type.

### Default Implementations

AppEnum Implementations

CaseDisplayRepresentable Implementations

Equatable Implementations

PersistentlyIdentifiable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- AppEnum
- AppValue
- CaseDisplayRepresentable
- CaseIterable
- CustomLocalizedStringResourceConvertible
- Equatable
- Hashable
- PersistentlyIdentifiable
- RawRepresentable
- Sendable
- StaticDisplayRepresentable
- TypeDisplayRepresentable

