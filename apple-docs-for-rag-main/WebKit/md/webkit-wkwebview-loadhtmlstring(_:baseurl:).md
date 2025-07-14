

- WebKit
- WKWebView
-  loadHTMLString(\_:baseURL:) 

Instance Method

# loadHTMLString(\_:baseURL:)

Loads the contents of the specified HTML string and navigates to it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
func loadHTMLString(
    _ string: String,
    baseURL: URL?
) -> WKNavigation?
```

## Parameters 

`string`  

The string to use as the contents of the webpage.

`baseURL`  

The base URL to use when the system resolves relative URLs within the HTML string.

## Return Value

A new navigation object you use to track the loading progress of the request.

## Discussion

Use this method to navigate to a webpage that you loaded or created yourself. For example, you might use this method to load HTML content that your app generates programmatically.

This method sets the source of this load request for app activity data to NSURLRequest.Attribution.developer.

## See Also

### Loading web content

func load(URLRequest) -> WKNavigation?

Loads the web content that the specified URL request object references and navigates to that content.

func load(Data, mimeType: String, characterEncodingName: String, baseURL: URL) -> WKNavigation?

Loads the content of the specified data object and navigates to it.

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

var estimatedProgress: Double

An estimate of what fraction of the current navigation has been loaded.

