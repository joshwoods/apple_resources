

- Foundation
- Locale
-  identifier(fromComponents:) 

Type Method

# identifier(fromComponents:)

Constructs an identifier from a dictionary of components.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func identifier(fromComponents components: [String : String]) -> String
```

## See Also

### Converting between identifiers

static func canonicalIdentifier(from: String) -> String

Returns a canonical identifier from the given string.

static func components(fromIdentifier: String) -> [String : String]

Returns a dictionary that splits an identifier into its component pieces.

Deprecated

static func identifier(Locale.IdentifierType, from: String) -> String

Returns the identifier conforming to the specified standard for the specified string.

enum IdentifierType

A type that indicates the standard that defines a locale’s identifier.

static func canonicalLanguageIdentifier(from: String) -> String

Returns a canonical language identifier from the given string.

static func identifier(fromWindowsLocaleCode: Int) -> String?

Returns the locale identifier from a given Windows locale code, or `nil` if it could not be converted.

static func windowsLocaleCode(fromIdentifier: String) -> Int?

Returns the Windows locale code from a given identifier, or `nil` if it could not be converted.

