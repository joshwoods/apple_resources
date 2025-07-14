

- Foundation
- Locale
-  Locale.IdentifierType 

Enumeration

# Locale.IdentifierType

A type that indicates the standard that defines a locale’s identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum IdentifierType
```

## Topics

### Standard Identifier Types

case icu

The type of identifiers that follow ICU (International Components for Unicode) conventions.

case cldr

The type of identifiers that follow CLDR (Common Locale Data Repository) conventions.

case bcp47

The type of BCP 47 language identifiers.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Converting between identifiers

static func canonicalIdentifier(from: String) -> String

Returns a canonical identifier from the given string.

static func components(fromIdentifier: String) -> [String : String]

Returns a dictionary that splits an identifier into its component pieces.

Deprecated

static func identifier(fromComponents: [String : String]) -> String

Constructs an identifier from a dictionary of components.

static func identifier(Locale.IdentifierType, from: String) -> String

Returns the identifier conforming to the specified standard for the specified string.

static func canonicalLanguageIdentifier(from: String) -> String

Returns a canonical language identifier from the given string.

static func identifier(fromWindowsLocaleCode: Int) -> String?

Returns the locale identifier from a given Windows locale code, or `nil` if it could not be converted.

static func windowsLocaleCode(fromIdentifier: String) -> Int?

Returns the Windows locale code from a given identifier, or `nil` if it could not be converted.

