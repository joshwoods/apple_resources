

- WebKit
- WKWebView
-  load(\_:mimeType:characterEncodingName:baseURL:) 

Instance Method

# load(\_:mimeType:characterEncodingName:baseURL:)

Loads the content of the specified data object and navigates to it.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
func load(
    _ data: Data,
    mimeType MIMEType: String,
    characterEncodingName: String,
    baseURL: URL
) -> WKNavigation?
```

## Parameters 

`data`  

The data to use as the contents of the webpage.

`MIMEType`  

The MIME type of the information in the `data` parameter. This parameter must not contain an empty string.

`characterEncodingName`  

The data’s character encoding name.

`baseURL`  

A URL that you use to resolve relative URLs within the document.

## Return Value

A new navigation object for tracking the request.

## Discussion

Use this method to navigate to a webpage that you loaded yourself and saved in a data object. For example, if you previously wrote HTML content to a data object, use this method to navigate to that content.

## See Also

### Loading web content

func load(URLRequest) -> WKNavigation?

Loads the web content that the specified URL request object references and navigates to that content.

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

var estimatedProgress: Double

An estimate of what fraction of the current navigation has been loaded.

