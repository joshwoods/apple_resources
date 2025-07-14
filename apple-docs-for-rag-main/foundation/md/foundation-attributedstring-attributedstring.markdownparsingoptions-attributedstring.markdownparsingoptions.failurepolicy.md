

- Foundation
- AttributedString
- AttributedString.MarkdownParsingOptions
-  AttributedString.MarkdownParsingOptions.FailurePolicy 

Enumeration

# AttributedString.MarkdownParsingOptions.FailurePolicy

A type that represents policies for handling parsing failures.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum FailurePolicy
```

## Topics

### Declaring Failure Policies

case returnPartiallyParsedIfPossible

A policy to return a partially-parsed string, if possible.

case throwError

A policy to throw an error from the initializer if parsing fails.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Options

var allowsExtendedAttributes: Bool

A Boolean value that indicates whether parsing allows extensions to Markdown that specify extended attributes.

var appliesSourcePositionAttributes: Bool

A Boolean value that indicates whether parsing applies attributes that indicate the position of attributed text in the original Markdown string.

var failurePolicy: AttributedString.MarkdownParsingOptions.FailurePolicy

The policy for handling a parsing failure.

var interpretedSyntax: AttributedString.MarkdownParsingOptions.InterpretedSyntax

The syntax for interpreting a Markdown string.

enum InterpretedSyntax

A type that represents the syntax for interpreting a Markdown string.

var languageCode: String?

The language code for this document.

