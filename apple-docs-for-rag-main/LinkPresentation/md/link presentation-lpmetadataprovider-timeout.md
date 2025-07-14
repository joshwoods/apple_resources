

- Link Presentation
- LPMetadataProvider
-  timeout 

Instance Property

# timeout

The time interval after which the request automatically fails if it hasn’t already completed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 18.0+visionOS 1.0+

``` source
var timeout: TimeInterval { get set }
```

## Discussion

The default timeout interval is 30 seconds. If a metadata fetch takes longer than the timeout interval, the completion handler is called with the error code LPError.Code.metadataFetchTimedOut.

## See Also

### Fetching metadata

func startFetchingMetadata(for: URL, completionHandler: (LPLinkMetadata?, (any Error)?) -> Void)

Fetches metadata for the given URL.

func cancel()

Cancels a metadata request.

var shouldFetchSubresources: Bool

A Boolean value indicating whether to download subresources specified by the metadata.

