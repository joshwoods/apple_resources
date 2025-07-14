

- Foundation
- Strings and Text
- AttributedString
-  Instantiating Attributed Strings with Markdown Syntax 

API Collection

# Instantiating Attributed Strings with Markdown Syntax

Use a Markdown-syntax string to iniitalize an attributed string with standard or custom attributes.

## Overview

You can use familiar Markdown syntax to initialize an attributed string with both its initial text and attributes for things like inline styles and links. In many cases, this produces easier-to-read code than manually setting attributes on ranges of an existing attributed string.

```
if let attString = try? AttributedString(
    markdown: "See the *latest* news at [our website](https://example.com)."),
    let websiteRange = attString.range(of: "our website"),
    let link = attString[websiteRange].link {
    print("\(link)") // Prints "https://example.com".
}
```

In this example, `attString` contains five runs, with attributes parsed from the syntax in the `markdown` parameter:

- `“See the “`, with no attributes.

- `“latest”`, with an AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute whose value is emphasized.

- `“ news at “`, with no attributes.

- `“our website”`, with an AttributeScopes.FoundationAttributes.LinkAttribute whose value is a URL.

- `“.”`, with no attributes.

You can also use custom attributes defined with the MarkdownDecodableAttributedStringKey protocol in the Markdown string. To do this, use Apple’s Markdown extension syntax: `^[text](attribute1: value1, attribute2: value2, …)`.

When using attributes beyond those provided by the system, be sure to use initializers that take a `scope` parameter, and provide the scope that defines the custom attributes.

Tip

The AttributedString initializers that take a `localized` parameter can also use Markdown syntax. These initializers allow you to use Markdown in your app’s strings files.

## Topics

### Initializing from Markdown Strings

init(markdown: String, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from a Markdown-formatted string using the provided options.

init&lt;S>(markdown: String, including: S.Type, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from a Markdown-formatted string using the provided options and attribute scope.

init&lt;S>(markdown: String, including: KeyPath&lt;AttributeScopes, S.Type>, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from a Markdown-formatted string using the provided options and attribute scope that a key path identifies.

### Initializing from Markdown Data

init(markdown: Data, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from Markdown-formatted data using the provided options.

init&lt;S>(markdown: Data, including: S.Type, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from Markdown-formatted data using the provided options and attribute scope.

init&lt;S>(markdown: Data, including: KeyPath&lt;AttributeScopes, S.Type>, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from Markdown-formatted data using the provided options and attribute scope that a key path identifies.

### Initializing with Markdown from URL Contents

init(contentsOf: URL, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from the contents of a specified URL that contains Markdown-formatted data, using the provided options.

init&lt;S>(contentsOf: URL, including: S.Type, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from the contents of a specified URL that contains Markdown-formatted data, using the provided options and attribute scope.

init&lt;S>(contentsOf: URL, including: KeyPath&lt;AttributeScopes, S.Type>, options: AttributedString.MarkdownParsingOptions, baseURL: URL?) throws

Creates an attributed string from the contents of a specified Markdown URL, using the provided options and attribute scope that a key path identifies.

### Specifying Markdown Parsing Options

struct MarkdownParsingOptions

Options that affect the parsing of Markdown content into an attributed string.

