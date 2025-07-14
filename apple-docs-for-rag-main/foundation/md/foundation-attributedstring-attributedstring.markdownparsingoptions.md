

- Foundation
- AttributedString
-  AttributedString.MarkdownParsingOptions 

Structure

# AttributedString.MarkdownParsingOptions

Options that affect the parsing of Markdown content into an attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MarkdownParsingOptions
```

## Topics

### Creating Markdown Parsing Options

init(allowsExtendedAttributes: Bool, interpretedSyntax: AttributedString.MarkdownParsingOptions.InterpretedSyntax, failurePolicy: AttributedString.MarkdownParsingOptions.FailurePolicy, languageCode: String?)

Creates a Markdown parsing options instance with the specified values.

init(allowsExtendedAttributes: Bool, interpretedSyntax: AttributedString.MarkdownParsingOptions.InterpretedSyntax, failurePolicy: AttributedString.MarkdownParsingOptions.FailurePolicy, languageCode: String?, appliesSourcePositionAttributes: Bool)

Creates a Markdown parsing options instance with the specified values, optionally marking the source position of attributed text.

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

enum InterpretedSyntax

A type that represents the syntax for interpreting a Markdown string.

var languageCode: String?

The language code for this document.

## Relationships

### Conforms To

- Copyable
- Sendable

