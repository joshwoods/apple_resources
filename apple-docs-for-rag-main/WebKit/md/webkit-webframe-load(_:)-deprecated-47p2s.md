

- WebKit
- WebFrame
-  load(\_:) Deprecated

Instance Method

# load(\_:)

Connects to a given URL by initiating an asynchronous client request.

macOS 10.3–10.14Deprecated

``` source
func load(_ request: URLRequest!)
```

## Parameters 

`request`  

A client request.

## Discussion

Creates a provisional data source that will transition to a committed data source once any data has been received. Use the dataSource method to check if a committed data source is available, and the stopLoading() method to stop the load. This method is typically invoked on the main frame.

## See Also

### Loading Content

func reload()

Reloads the initial request passed as an argument to load(_:).

Deprecated

func reloadFromOrigin()

Performs an end-to-end revalidation using cache-validating conditionals if possible.

Deprecated

func stopLoading()

Stops any pending loads on the receiver’s data source, and those of its children.

Deprecated

func loadAlternateHTMLString(String!, baseURL: URL!, forUnreachableURL: URL!)

Loads alternate content for a frame whose URL is unreachable.

Deprecated

func loadHTMLString(String!, baseURL: URL!)

Sets the main page contents and base URL.

Deprecated

func load(Data!, mimeType: String!, textEncodingName: String!, baseURL: URL!)

Sets the main page contents, MIME type, content encoding, and base URL.

Deprecated

func load(WebArchive!)

Loads an archive into the web frame.

Deprecated

