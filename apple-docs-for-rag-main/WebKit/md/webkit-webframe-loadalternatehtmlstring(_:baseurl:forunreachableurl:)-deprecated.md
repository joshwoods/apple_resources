

- WebKit
- WebFrame
-  loadAlternateHTMLString(\_:baseURL:forUnreachableURL:) Deprecated

Instance Method

# loadAlternateHTMLString(\_:baseURL:forUnreachableURL:)

Loads alternate content for a frame whose URL is unreachable.

macOS 10.3–10.14Deprecated

``` source
func loadAlternateHTMLString(
    _ string: String!,
    baseURL: URL!,
    forUnreachableURL unreachableURL: URL!
)
```

## Parameters 

`string`  

The string to use as the main page for the document.

`baseURL`  

A file that is used to resolve relative URLs within the document.

`unreachableURL`  

The URL for the alternate page content.

## Discussion

Use this method to display page-level loading errors in a web view. Typically, a `WebFrameLoadDelegate` or `WebPolicyDelegate` object invokes this method from these methods: `webView:didFailProvisionalLoadWithError:forFrame:` (`WebFrameLoadDelegate`), webView:decidePolicyForMIMEType:request:frame:decisionListener: (`WebPolicyDelegate`), or webView(_:unableToImplementPolicyWithError:frame:) (`WebPolicyDelegate`). If invoked from one of these methods, the back-forward list is maintained.

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

func loadHTMLString(String!, baseURL: URL!)

Sets the main page contents and base URL.

Deprecated

func load(Data!, mimeType: String!, textEncodingName: String!, baseURL: URL!)

Sets the main page contents, MIME type, content encoding, and base URL.

Deprecated

func load(WebArchive!)

Loads an archive into the web frame.

Deprecated

