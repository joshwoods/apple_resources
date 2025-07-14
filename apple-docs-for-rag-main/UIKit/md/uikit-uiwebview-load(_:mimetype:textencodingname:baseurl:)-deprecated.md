

- UIKit
- UIWebView
-  load(\_:mimeType:textEncodingName:baseURL:) Deprecated

Instance Method

# load(\_:mimeType:textEncodingName:baseURL:)

Sets the main page contents, MIME type, content encoding, and base URL.

iOS 2.0–12.0DeprecatediPadOS 2.0–12.0Deprecated

``` source
@MainActor
func load(
    _ data: Data,
    mimeType MIMEType: String,
    textEncodingName: String,
    baseURL: URL
)
```

## Parameters 

`data`  

The content for the main page.

`MIMEType`  

The MIME type of the content.

`textEncodingName`  

The IANA encoding name as in `utf-8` or `utf-16`.

`baseURL`  

The base URL for the content.

## See Also

### Loading content

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

func stopLoading()

Stops the loading of any web content managed by the receiver.

Deprecated

func reload()

Reloads the current page.

Deprecated

