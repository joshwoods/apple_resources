

- WebKit
- WebDataSource
-  representation Deprecated

Instance Property

# representation

The data source’s representation depending on its MIME type.

macOS 10.3–10.14Deprecated

``` source
var representation: (any WebDocumentRepresentation)! { get }
```

## Discussion

`nil` if the data source is in the process of being loaded and this method is invoked before loading is complete.

You can specify the mapping between a representation and MIME type using the \`\`WebView/registerClass(\_:representationClass:forMIMEType:)\`\`\`WebView\` class method.

## See Also

### Querying page data and state

var data: Data!

The raw data that represents the data source’s content.

Deprecated

var isLoading: Bool

A Boolean that indicates whether the data source is loading its content.

Deprecated

var pageTitle: String!

The title of the data source’s page.

Deprecated

var textEncodingName: String!

The text encoding for the data source’s web view, if set, or the text encoding of the response.

Deprecated

