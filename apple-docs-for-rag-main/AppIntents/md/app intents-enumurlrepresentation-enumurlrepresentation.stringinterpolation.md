

- App Intents
- EnumURLRepresentation
-  EnumURLRepresentation.StringInterpolation 

Structure

# EnumURLRepresentation.StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct StringInterpolation
```

Available when `Enum` conforms to `AppEnum`.

## Overview

The `StringLiteralType` of an interpolation type must match the `StringLiteralType` of the conforming type.

## Topics

### Initializers

init(literalCapacity: Int, interpolationCount: Int)

Creates an empty instance ready to be filled with string literal content.

### Instance Methods

func appendInterpolation(Enum)

func appendInterpolation(EnumURLRepresentation&lt;Enum>.StringInterpolation.Token)

func appendLiteral(String)

Appends a literal segment to the interpolation.

### Type Aliases

typealias StringLiteralType

The type that should be used for literal segments.

### Enumerations

enum Token

## Relationships

### Conforms To

- StringInterpolationProtocol

