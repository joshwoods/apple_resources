

- App Intents
-  ParameterSummaryString 

Structure

# ParameterSummaryString

A human-readable string that interpolates parameter key paths to provide user-configurable placeholders in the Shortcuts app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ParameterSummaryString where Intent : AppIntent
```

## Topics

### Creating the summary string

init(String)

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(stringInterpolation: ParameterSummaryString&lt;Intent>.StringInterpolation)

Creates an instance from a string interpolation.

struct StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

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

### Shortcuts support

protocol ParameterSummary

An interface for defining the visual representation of an app intent’s parameters.

struct IntentParameterSummary

A type that describes the user interface configuration of an app intent’s parameters.

struct ParameterSummaryWhenCondition

A type that represents a conditional statement in a parameter summary.

struct ParameterSummarySwitchCondition

A type that represents a switch statement in a parameter summary.

struct ParameterSummaryCaseCondition

A type that represents an individual case of a switch statement in a parameter summary.

struct ParameterSummaryDefaultCaseCondition

A type that represents the default case of a switch statement in a parameter summary.

