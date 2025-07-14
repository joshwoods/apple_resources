

- WebKit
- WebFrame
-  loadHTMLString(\_:baseURL:) Deprecated

Instance Method

# loadHTMLString(\_:baseURL:)

Sets the main page contents and base URL.

macOS 10.3–10.14Deprecated

``` source
func loadHTMLString(
    _ string: String!,
    baseURL URL: URL!
)
```

## Parameters 

`string`  

The string to use as the main page for the document.

Since the string is treated as a webpage with UTF-8 encoding, the default encoding for any script elements referenced by the HTML is also UTF-8. To avoid this, include a character set attribute on the script element.

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

func load(Data!, mimeType: String!, textEncodingName: String!, baseURL: URL!)

Sets the main page contents, MIME type, content encoding, and base URL.

Deprecated

func load(WebArchive!)

Loads an archive into the web frame.

Deprecated

