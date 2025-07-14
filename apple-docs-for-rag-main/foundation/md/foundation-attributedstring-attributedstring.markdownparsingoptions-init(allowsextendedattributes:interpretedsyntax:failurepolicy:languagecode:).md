

- Foundation
- AttributedString
- AttributedString.MarkdownParsingOptions
-  init(allowsExtendedAttributes:interpretedSyntax:failurePolicy:languageCode:) 

Initializer

# init(allowsExtendedAttributes:interpretedSyntax:failurePolicy:languageCode:)

Creates a Markdown parsing options instance with the specified values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    allowsExtendedAttributes: Bool = false,
    interpretedSyntax: AttributedString.MarkdownParsingOptions.InterpretedSyntax = .full,
    failurePolicy: AttributedString.MarkdownParsingOptions.FailurePolicy = .throwError,
    languageCode: String? = nil
)
```

## Parameters 

`allowsExtendedAttributes`  

A Boolean value that indicates whether parsing allows extensions to Markdown that specify extended attributes.

`interpretedSyntax`  

The syntax for intepreting a Markdown string.

`failurePolicy`  

The policy for handling a parsing failure.

`languageCode`  

The BCP-47 language code for this document.

## See Also

### Creating Markdown Parsing Options

init(allowsExtendedAttributes: Bool, interpretedSyntax: AttributedString.MarkdownParsingOptions.InterpretedSyntax, failurePolicy: AttributedString.MarkdownParsingOptions.FailurePolicy, languageCode: String?, appliesSourcePositionAttributes: Bool)

Creates a Markdown parsing options instance with the specified values, optionally marking the source position of attributed text.

