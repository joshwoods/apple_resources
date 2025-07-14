

- Foundation
- AttributedString
- AttributedString.MarkdownParsingOptions
-  allowsExtendedAttributes 

Instance Property

# allowsExtendedAttributes

A Boolean value that indicates whether parsing allows extensions to Markdown that specify extended attributes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var allowsExtendedAttributes: Bool
```

## Discussion

If this value is `false`, the Markdown parser supports only the CommonMark syntax. The default is `false`.

## See Also

### Accessing Options

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

