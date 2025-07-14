

- UIKit
- UIWebView
-  stopLoading() Deprecated

Instance Method

# stopLoading()

Stops the loading of any web content managed by the receiver.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
func stopLoading()
```

## Discussion

Stops any content in the process of being loaded by the main frame or any of its children frames. Does nothing if no content is being loaded.

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

var request: URLRequest?

The URL request identifying the location of the content to load.

Deprecated

var isLoading: Bool

A Boolean value indicating whether the receiver is done loading content.

Deprecated

func reload()

Reloads the current page.

Deprecated

