

- WebKit
- WebDataSource
-  isLoading Deprecated

Instance Property

# isLoading

A Boolean that indicates whether the data source is loading its content.

macOS 10.3–10.14Deprecated

``` source
var isLoading: Bool { get }
```

## Discussion

true if the data source is in the process of loading its content; otherwise, false.

## See Also

### Querying page data and state

var data: Data!

The raw data that represents the data source’s content.

Deprecated

var pageTitle: String!

The title of the data source’s page.

Deprecated

var representation: (any WebDocumentRepresentation)!

The data source’s representation depending on its MIME type.

Deprecated

var textEncodingName: String!

The text encoding for the data source’s web view, if set, or the text encoding of the response.

Deprecated

