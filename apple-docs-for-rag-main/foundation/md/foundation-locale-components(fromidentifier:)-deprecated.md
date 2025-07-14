

- Foundation
- Locale
-  components(fromIdentifier:) Deprecated

Type Method

# components(fromIdentifier:)

Returns a dictionary that splits an identifier into its component pieces.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 8.0–16.0DeprecatedmacOS 10.10–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0+watchOS 2.0–9.0Deprecated

``` source
static func components(fromIdentifier string: String) -> [String : String]
```

Deprecated

Use \`Locale.Components(identifier:)\` to access components

## See Also

### Converting between identifiers

static func canonicalIdentifier(from: String) -> String

Returns a canonical identifier from the given string.

static func identifier(fromComponents: [String : String]) -> String

Constructs an identifier from a dictionary of components.

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

