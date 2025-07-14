

- App Intents
- AppShortcutParameterPresentationSummaryString
-  AppShortcutParameterPresentationSummaryString.StringInterpolation 

Structure

# AppShortcutParameterPresentationSummaryString.StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

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

func appendInterpolation(ParameterKeyPath)

func appendLiteral(String)

Appends a literal segment to the interpolation.

### Type Aliases

typealias StringLiteralType

The type that should be used for literal segments.

## Relationships

### Conforms To

- StringInterpolationProtocol

