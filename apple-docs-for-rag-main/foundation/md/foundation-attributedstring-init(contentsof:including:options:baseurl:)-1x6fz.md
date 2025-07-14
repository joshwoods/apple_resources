

- Foundation
- AttributedString
-  init(contentsOf:including:options:baseURL:) 

Initializer

# init(contentsOf:including:options:baseURL:)

Creates an attributed string from the contents of a specified URL that contains Markdown-formatted data, using the provided options and attribute scope.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    contentsOf url: URL,
    including scope: S.Type,
    options: AttributedString.MarkdownParsingOptions = .init(),
    baseURL: URL? = nil
) throws where S : AttributeScope
```

## Parameters 

`url`  

The URL to load Markdown-formatted data from.

`scope`  

An attribute scope to associate with the attributed string.

`options`  

Options that affect how the initializer interprets formatting in the Markdown string. This parameter defaults to no options.

`baseURL`  

The base URL to use when resolving Markdown URLs. The initializer treats URLs as being relative to this URL. If this value is `nil`, the initializer doesn’t resolve URLs. The default is `nil`.

## Discussion

If your source string includes custom attributes defined by conformers to MarkdownDecodableAttributedStringKey and used with Apple’s markdown extension syntax, be sure to include the allowsExtendedAttributes option. Otherwise, the initializer doesn’t parse these attributes.

## See Also

### Initializing with Markdown from URL Contents

init(contentsOf: URL, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from the contents of a specified URL that contains Markdown-formatted data, using the provided options.

init&lt;S>(contentsOf: URL, including: KeyPath&lt;AttributeScopes, S.Type>, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from the contents of a specified Markdown URL, using the provided options and attribute scope that a key path identifies.

