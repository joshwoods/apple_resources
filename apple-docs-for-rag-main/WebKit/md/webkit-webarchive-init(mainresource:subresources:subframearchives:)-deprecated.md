

- WebKit
- WebArchive
-  init(mainResource:subresources:subframeArchives:) Deprecated

Initializer

# init(mainResource:subresources:subframeArchives:)

Initializes the receiver with a resource and optional subresources and subframe archives..

macOS 10.3–10.14Deprecated

``` source
init!(
    mainResource: WebResource!,
    subresources: [Any]!,
    subframeArchives: [Any]!
)
```

## Discussion

This method initializes and returns the receiver by setting the main resource to `mainResource`, and setting the subresources and subframe archives if supplied. The `subresources` argument should be an array of WebResource objects or `nil` if none are specified. The `subframeArchives` should be and array of WebArchive objects used by the subframes or `nil` if none are specified.

## See Also

### Initializing

init!(data: Data!)

Initializes and returns the receiver, specifying the initial content data.

Deprecated

