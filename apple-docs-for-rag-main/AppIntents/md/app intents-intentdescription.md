

- App Intents
-  IntentDescription 

Structure

# IntentDescription

The human-readable description and metadata for an app intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentDescription
```

## Topics

### Creating a description

init(LocalizedStringResource, categoryName: LocalizedStringResource?, searchKeywords: [LocalizedStringResource])

### Initializers

init(LocalizedStringResource, categoryName: LocalizedStringResource?, searchKeywords: [LocalizedStringResource], resultValueName: LocalizedStringResource?)

init(stringLiteral: String)

Creates an instance initialized to the given string value.

### Instance Properties

var categoryName: LocalizedStringResource?

The category in which this intent will be grouped into in the Shortcuts editor.

var descriptionText: LocalizedStringResource

A short, localized, human-readable string that describes the intent using sentence case and followed by a period.

var resultValueName: LocalizedStringResource?

A name for the result of this intent, which will be displayed in the Shortcuts editor, such as when the output is used as a variable.

var searchKeywords: [LocalizedStringResource]

A set of keywords which, when searched in the Shortcuts editor, will reveal this intent.

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
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Sendable

## See Also

### Supplementary content

protocol AppIntentsPackage

A type that describes app intent definitions that aren’t part of an app bundle and their dependencies.

struct IntentDialog

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

struct IntentDeprecation

class IntentProjection

Projections for an app intent that returns non-optional values for parameters.

struct IntentSystemContext

Information that the system makes available to an app intent while it performs its action.

