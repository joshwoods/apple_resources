

- WebKit
- WKWebView
-  loadSimulatedRequest(\_:response:responseData:) 

Instance Method

# loadSimulatedRequest(\_:response:responseData:)

Loads the web content from the data you provide as if the data were the response to the request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
func loadSimulatedRequest(
    _ request: URLRequest,
    response: URLResponse,
    responseData data: Data
) -> WKNavigation
```

## Parameters 

`request`  

A URL request that specifies the base URL and other loading details the system uses to interpret the data you provide.

`response`  

A response the system uses to interpret the data you provide.

`data`  

The data to use as the contents of the webpage.

## Return Value

A new navigation object you use to track the loading progress of the request.

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

func loadSimulatedRequest(URLRequest, responseHTML: String) -> WKNavigation

Loads the web content from the HTML you provide as if the HTML were the response to the request.

var isLoading: Bool

A Boolean value that indicates whether the view is currently loading content.

var estimatedProgress: Double

An estimate of what fraction of the current navigation has been loaded.

