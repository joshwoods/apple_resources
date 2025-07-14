

- App Intents
-  StringSearchScope 

Enumeration

# StringSearchScope

Constants that help the system understand the in-app search functionality and its searchable content.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
enum StringSearchScope
```

## Topics

### Search scopes

case freeformVideo

The app supports searching for free-form video content like videos people upload to social media platforms.

case general

The app offers a general search functionality that’s exposed to the system.

case movies

The app supports searching for structured movie content.

case tv

The app supports searching for structured TV content including shows, seasons, or episodes.

### Providing descriptions

static var caseDisplayRepresentations: [StringSearchScope : DisplayRepresentation]

A dictionary that maps each value to the visual elements that represent it.

static var typeDisplayRepresentation: TypeDisplayRepresentation

A short, localized, human-readable name for the type.

### Creating a search scope

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

static var allCases: [StringSearchScope]

A collection of all values of this type.

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

## See Also

### Scoping the search

static var searchScopes: Self.Criteria.SearchScopes

Values that help the system understand the scope of an app intent that shows the results of a string-based search.

**Required** Default implementations provided.

