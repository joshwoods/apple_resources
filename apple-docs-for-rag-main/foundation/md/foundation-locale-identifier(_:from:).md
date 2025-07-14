

- Foundation
- Locale
-  identifier(\_:from:) 

Type Method

# identifier(\_:from:)

Returns the identifier conforming to the specified standard for the specified string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func identifier(
    _ type: Locale.IdentifierType,
    from string: String
) -> String
```

## Parameters 

`type`  

The identifier type used by `string`, such as Locale.IdentifierType.icu or Locale.IdentifierType.bcp47.

`string`  

An identifier string that complies with the standard indicated by `type`.

## Return Value

A locale identifier.

## See Also

### Converting between identifiers

static func canonicalIdentifier(from: String) -> String

Returns a canonical identifier from the given string.

static func components(fromIdentifier: String) -> [String : String]

Returns a dictionary that splits an identifier into its component pieces.

Deprecated

static func identifier(fromComponents: [String : String]) -> String

Constructs an identifier from a dictionary of components.

enum IdentifierType

A type that indicates the standard that defines a locale’s identifier.

static func canonicalLanguageIdentifier(from: String) -> String

Returns a canonical language identifier from the given string.

static func identifier(fromWindowsLocaleCode: Int) -> String?

Returns the locale identifier from a given Windows locale code, or `nil` if it could not be converted.

static func windowsLocaleCode(fromIdentifier: String) -> Int?

Returns the Windows locale code from a given identifier, or `nil` if it could not be converted.

