

- WebKit
- WebFrame
-  load(\_:mimeType:textEncodingName:baseURL:) Deprecated

Instance Method

# load(\_:mimeType:textEncodingName:baseURL:)

Sets the main page contents, MIME type, content encoding, and base URL.

macOS 10.3–10.14Deprecated

``` source
func load(
    _ data: Data!,
    mimeType MIMEType: String!,
    textEncodingName encodingName: String!,
    baseURL URL: URL!
)
```

## Parameters 

`data`  

The data to use for the main page of the document.

`MIMEType`  

The MIME type of the data.

`encodingName`  

The IANA encoding name (for example, “utf-8” or “utf-16”).

`URL`  

A file that is used to resolve relative URLs within the document.

## See Also

### Loading Content

func load(URLRequest!)

Connects to a given URL by initiating an asynchronous client request.

Deprecated

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

func load(WebArchive!)

Loads an archive into the web frame.

Deprecated

