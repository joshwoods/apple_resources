

- Foundation
- AttributedString
- AttributedString.MarkdownParsingOptions
-  appliesSourcePositionAttributes 

Instance Property

# appliesSourcePositionAttributes

A Boolean value that indicates whether parsing applies attributes that indicate the position of attributed text in the original Markdown string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var appliesSourcePositionAttributes: Bool
```

## See Also

### Accessing Options

var allowsExtendedAttributes: Bool

A Boolean value that indicates whether parsing allows extensions to Markdown that specify extended attributes.

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

