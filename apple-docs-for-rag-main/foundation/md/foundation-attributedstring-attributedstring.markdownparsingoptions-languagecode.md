

- Foundation
- AttributedString
- AttributedString.MarkdownParsingOptions
-  languageCode 

Instance Property

# languageCode

The language code for this document.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var languageCode: String?
```

## Discussion

This value is a BCP-47 language code. If not `nil`, the string applies the languageIdentifier attribute to any range in the returned string that doesn’t otherwise specify a language attribute. The default is `nil`, which applies no attributes.

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

enum InterpretedSyntax

A type that represents the syntax for interpreting a Markdown string.

