

- App Intents
-  IntentDialog 

Structure

# IntentDialog

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentDialog
```

## Topics

### Creating a dialog

init(LocalizedStringResource)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(stringInterpolation: String.LocalizationValue.StringInterpolation)

Creates an instance from a string interpolation.

init(full: LocalizedStringResource, supporting: LocalizedStringResource)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

### Initializers

init(full: LocalizedStringResource, supporting: LocalizedStringResource, systemImageName: String)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

init(full: LocalizedStringResource, systemImageName: String)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

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
- Sendable

## See Also

### Supplementary content

protocol AppIntentsPackage

A type that describes app intent definitions that aren’t part of an app bundle and their dependencies.

struct IntentDescription

The human-readable description and metadata for an app intent.

struct IntentDeprecation

class IntentProjection

Projections for an app intent that returns non-optional values for parameters.

struct IntentSystemContext

Information that the system makes available to an app intent while it performs its action.

