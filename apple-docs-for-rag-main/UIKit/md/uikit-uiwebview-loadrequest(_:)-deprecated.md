

- UIKit
- UIWebView
-  loadRequest(\_:) Deprecated

Instance Method

# loadRequest(\_:)

Connects to a given URL by initiating an asynchronous client request.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
func loadRequest(_ request: URLRequest)
```

## Parameters 

`request`  

A URL request identifying the location of the content to load.

## Discussion

Don’t use this method to load local HTML files; instead, use loadHTMLString(_:baseURL:). To stop this load, use the stopLoading() method. To see whether the receiver is done loading the content, use the isLoading property.

## See Also

### Loading content

func load(Data, mimeType: String, textEncodingName: String, baseURL: URL)

Sets the main page contents, MIME type, content encoding, and base URL.

Deprecated

func loadHTMLString(String, baseURL: URL?)

Sets the main page content and base URL.

Deprecated

var request: URLRequest?

The URL request identifying the location of the content to load.

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

