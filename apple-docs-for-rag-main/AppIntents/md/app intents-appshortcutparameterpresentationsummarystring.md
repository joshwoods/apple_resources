

- App Intents
-  AppShortcutParameterPresentationSummaryString 

Structure

# AppShortcutParameterPresentationSummaryString

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AppShortcutParameterPresentationSummaryString where Intent : AppIntent, Value : _IntentValue, Value : Sendable, Parameter : IntentParameter, ParameterKeyPath : KeyPath
```

## Topics

### Structures

struct StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

### Initializers

init(String)

init(stringInterpolation: AppShortcutParameterPresentationSummaryString&lt;Intent, Value, Parameter, ParameterKeyPath>.StringInterpolation)

Creates an instance from a string interpolation.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Default Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

## See Also

### App Shortcut parameter presentation

struct AppShortcutParameterPresentation

Describes the presentation of an App Shortcut for the provided parameter.

struct AppShortcutParameterPresentationSummary

The summary of the presentation of an App Shortcut parameter.

struct AppShortcutParameterPresentationTitle

A struct that represents the title of the presentation of an App Shortcut.

Deprecated

struct AppShortcutParameterPresentationTitleStringDeprecated

