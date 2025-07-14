

- App Intents
- NegativeAppShortcutPhrase
-  NegativeAppShortcutPhrase.StringInterpolation 

Structure

# NegativeAppShortcutPhrase.StringInterpolation

A string you construct using literal values, content from intent parameters, and other interpolated values.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct StringInterpolation
```

## Topics

### Initializers

init(literalCapacity: Int, interpolationCount: Int)

Creates an empty instance ready to be filled with string literal content.

### Instance Methods

func appendInterpolation(AppShortcutPhraseToken)

func appendLiteral(String)

Appends a literal segment to the interpolation.

### Type Aliases

typealias StringLiteralType

The type that should be used for literal segments.

## Relationships

### Conforms To

- StringInterpolationProtocol

