

- Foundation
- NSAttributedString
-  init(markdown:options:baseURL:) 

Initializer

# init(markdown:options:baseURL:)

Creates an attributed string from Markdown-formatted data using the provided options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(
    markdown: Data,
    options: AttributedString.MarkdownParsingOptions = .init(),
    baseURL: URL? = nil
) throws
```

## Parameters 

`markdown`  

The Data instance that contains the Markdown formatting.

`options`  

Options that affect how the initializer interprets formatting in the Markdown string. This parameter defaults to no options.

`baseURL`  

The base URL to use when resolving Markdown URLs. The initializer treats URLs as being relative to this URL. If this value is `nil`, the initializer doesn’t resolve URLs. The default is `nil`.

## See Also

### Creating from markdown

convenience init(markdown: String, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from a Markdown-formatted string using the provided options.

convenience init(contentsOf: URL, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from the contents of a specified URL that contains Markdown-formatted data using the provided options.

