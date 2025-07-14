

- Foundation
- AttributedString
-  init(markdown:including:options:baseURL:) 

Initializer

# init(markdown:including:options:baseURL:)

Creates an attributed string from Markdown-formatted data using the provided options and attribute scope that a key path identifies.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    markdown: Data,
    including scope: KeyPath,
    options: AttributedString.MarkdownParsingOptions = .init(),
    baseURL: URL? = nil
) throws where S : AttributeScope
```

## Parameters 

`markdown`  

The Data instance that contains the Markdown formatting.

`scope`  

The AttributeScopes key path that identifies an attribute scope to associate with the attributed string.

`options`  

Options that affect how the initializer interprets formatting in the Markdown string. This parameter defaults to no options.

`baseURL`  

The base URL to use when resolving Markdown URLs. The initializer treats URLs as being relative to this URL. If this value is `nil`, the initializer doesn’t resolve URLs. The default is `nil`.

## Discussion

If your source string includes custom attributes defined by conformers to MarkdownDecodableAttributedStringKey and used with Apple’s markdown extension syntax, be sure to include the allowsExtendedAttributes option. Otherwise, the initializer doesn’t parse these attributes.

## See Also

### Initializing from Markdown Data

init(markdown: Data, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from Markdown-formatted data using the provided options.

init&lt;S>(markdown: Data, including: S.Type, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from Markdown-formatted data using the provided options and attribute scope.

