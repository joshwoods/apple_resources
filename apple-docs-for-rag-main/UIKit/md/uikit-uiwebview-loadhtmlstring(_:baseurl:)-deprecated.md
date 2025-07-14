

- UIKit
- UIWebView
-  loadHTMLString(\_:baseURL:) Deprecated

Instance Method

# loadHTMLString(\_:baseURL:)

Sets the main page content and base URL.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
func loadHTMLString(
    _ string: String,
    baseURL: URL?
)
```

## Parameters 

`string`  

The content for the main page.

`baseURL`  

The base URL for the content.

## Discussion

To help you avoid being vulnerable to security attacks, be sure to use this method to load local HTML files; don’t use loadRequest(_:).

## See Also

### Loading content

func load(Data, mimeType: String, textEncodingName: String, baseURL: URL)

Sets the main page contents, MIME type, content encoding, and base URL.

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

func stopLoading()

Stops the loading of any web content managed by the receiver.

Deprecated

func reload()

Reloads the current page.

Deprecated

