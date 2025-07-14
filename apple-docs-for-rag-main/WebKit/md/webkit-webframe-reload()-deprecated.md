

- WebKit
- WebFrame
-  reload() Deprecated

Instance Method

# reload()

Reloads the initial request passed as an argument to load(_:).

macOS 10.3–10.14Deprecated

``` source
func reload()
```

## See Also

### Loading Content

func load(URLRequest!)

Connects to a given URL by initiating an asynchronous client request.

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

