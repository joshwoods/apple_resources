

- Foundation
- AttributedString
- AttributedString.MarkdownParsingOptions
-  AttributedString.MarkdownParsingOptions.InterpretedSyntax 

Enumeration

# AttributedString.MarkdownParsingOptions.InterpretedSyntax

A type that represents the syntax for interpreting a Markdown string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum InterpretedSyntax
```

## Topics

### Syntax Values

case full

A syntax value that interprets the full Markdown syntax and produces all relevant attributes.

case inlineOnly

A syntax value that parses all Markdown text, but interprets only attributes that apply to inline spans.

case inlineOnlyPreservingWhitespace

A syntax value that parses all Markdown text, but interprets only attributes that apply to inline spans, preserving white space.

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

enum FailurePolicy

A type that represents policies for handling parsing failures.

var interpretedSyntax: AttributedString.MarkdownParsingOptions.InterpretedSyntax

The syntax for interpreting a Markdown string.

var languageCode: String?

The language code for this document.

