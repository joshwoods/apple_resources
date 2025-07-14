

- WebKit
- WebDataSource
-  pageTitle Deprecated

Instance Property

# pageTitle

The title of the data source’s page.

macOS 10.3–10.14Deprecated

``` source
var pageTitle: String! { get }
```

## Discussion

The associated web view notifies its frame load delegate when the page title is loaded by invoking the `webView:didReceiveTitle:forFrame:` delegate method.

`nil` if the page has no title or the page title hasn’t been loaded yet.

## See Also

### Querying page data and state

var data: Data!

The raw data that represents the data source’s content.

Deprecated

var isLoading: Bool

A Boolean that indicates whether the data source is loading its content.

Deprecated

var representation: (any WebDocumentRepresentation)!

The data source’s representation depending on its MIME type.

Deprecated

var textEncodingName: String!

The text encoding for the data source’s web view, if set, or the text encoding of the response.

Deprecated

