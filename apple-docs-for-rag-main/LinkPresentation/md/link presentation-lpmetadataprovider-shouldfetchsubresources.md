

- Link Presentation
- LPMetadataProvider
-  shouldFetchSubresources 

Instance Property

# shouldFetchSubresources

A Boolean value indicating whether to download subresources specified by the metadata.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 18.0+visionOS 1.0+

``` source
var shouldFetchSubresources: Bool { get set }
```

## Discussion

Subresources include the icon, image, or video. When set to `false`, the returned LPLinkMetadata object consists only of metadata retrieved from the main resource identified by the url passed to startFetchingMetadata(for:completionHandler:).

The default value is `true`.

## See Also

### Fetching metadata

func startFetchingMetadata(for: URL, completionHandler: (LPLinkMetadata?, (any Error)?) -> Void)

Fetches metadata for the given URL.

func cancel()

Cancels a metadata request.

var timeout: TimeInterval

The time interval after which the request automatically fails if it hasn’t already completed.

