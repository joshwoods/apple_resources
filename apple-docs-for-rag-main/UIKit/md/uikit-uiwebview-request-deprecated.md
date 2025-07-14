

- UIKit
- UIWebView
-  request Deprecated

Instance Property

# request

The URL request identifying the location of the content to load.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
var request: URLRequest? { get }
```

## See Also

### Loading content

func load(Data, mimeType: String, textEncodingName: String, baseURL: URL)

Sets the main page contents, MIME type, content encoding, and base URL.

Deprecated

func loadHTMLString(String, baseURL: URL?)

Sets the main page content and base URL.

Deprecated

func loadRequest(URLRequest)

Connects to a given URL by initiating an asynchronous client request.

Deprecated

var isLoading: Bool

A Boolean value indicating whether the receiver is done loading content.

Deprecated

func stopLoading()

Stops the loading of any web content managed by the receiver.

Deprecated

func reload()

Reloads the current page.

Deprecated

