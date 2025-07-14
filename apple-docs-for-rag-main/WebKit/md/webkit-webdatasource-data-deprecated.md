

- WebKit
- WebDataSource
-  data Deprecated

Instance Property

# data

The raw data that represents the data source’s content.

macOS 10.3–10.14Deprecated

``` source
var data: Data! { get }
```

## Discussion

The format of the data is dependent on the data source’s MIME type (obtained from the response).

## See Also

### Querying page data and state

var isLoading: Bool

A Boolean that indicates whether the data source is loading its content.

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

