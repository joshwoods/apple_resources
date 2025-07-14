

- WebKit
- WKWebView
-  estimatedProgress 

Instance Property

# estimatedProgress

An estimate of what fraction of the current navigation has been loaded.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var estimatedProgress: Double { get }
```

## Discussion

This value ranges from `0.0` to `1.0` based on the total number of bytes received, including the main document and all of its potential subresources. After navigation loading completes, the `estimatedProgress` value remains at `1.0` until a new navigation starts, at which point the `estimatedProgress` value resets to `0.0`. The WKWebView class is key-value observing (KVO) compliant for this property.

## See Also

### Loading web content

func load(URLRequest) -> WKNavigation?

Loads the web content that the specified URL request object references and navigates to that content.

func load(Data, mimeType: String, characterEncodingName: String, baseURL: URL) -> WKNavigation?

Loads the content of the specified data object and navigates to it.

func loadHTMLString(String, baseURL: URL?) -> WKNavigation?

Loads the contents of the specified HTML string and navigates to it.

func loadFileRequest(URLRequest, allowingReadAccessTo: URL) -> WKNavigation

Loads the web content from the file the URL request object specifies and navigates to that content.

func loadFileURL(URL, allowingReadAccessTo: URL) -> WKNavigation?

Loads the web content from the specified file and navigates to it.

func loadSimulatedRequest(URLRequest, response: URLResponse, responseData: Data) -> WKNavigation

Loads the web content from the data you provide as if the data were the response to the request.

func loadSimulatedRequest(URLRequest, responseHTML: String) -> WKNavigation

Loads the web content from the HTML you provide as if the HTML were the response to the request.

var isLoading: Bool

A Boolean value that indicates whether the view is currently loading content.

