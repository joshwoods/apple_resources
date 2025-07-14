

- App Intents
- ParameterSummaryString
-  ParameterSummaryString.StringInterpolation 

Structure

# ParameterSummaryString.StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct StringInterpolation
```

## Overview

The `StringLiteralType` of an interpolation type must match the `StringLiteralType` of the conforming type.

## Topics

### Initializers

init(literalCapacity: Int, interpolationCount: Int)

Creates an empty instance ready to be filled with string literal content.

### Instance Methods

func appendInterpolation&lt;ValueType, Subject>(Subject)

func appendLiteral(String)

Appends a literal segment to the interpolation.

### Type Aliases

typealias StringLiteralType

The type that should be used for literal segments.

## Relationships

### Conforms To

- StringInterpolationProtocol

## See Also

### Creating the summary string

init(String)

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(stringInterpolation: ParameterSummaryString&lt;Intent>.StringInterpolation)

Creates an instance from a string interpolation.

