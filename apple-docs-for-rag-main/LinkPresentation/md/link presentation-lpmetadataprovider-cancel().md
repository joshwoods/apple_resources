

- Link Presentation
- LPMetadataProvider
-  cancel() 

Instance Method

# cancel()

Cancels a metadata request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 18.0+visionOS 1.0+

``` source
func cancel()
```

## Discussion

This method invokes the completion handler with the error code LPError.Code.metadataFetchCancelled if the request hasn’t already completed.

## See Also

### Fetching metadata

func startFetchingMetadata(for: URL, completionHandler: (LPLinkMetadata?, (any Error)?) -> Void)

Fetches metadata for the given URL.

var shouldFetchSubresources: Bool

A Boolean value indicating whether to download subresources specified by the metadata.

var timeout: TimeInterval

The time interval after which the request automatically fails if it hasn’t already completed.

