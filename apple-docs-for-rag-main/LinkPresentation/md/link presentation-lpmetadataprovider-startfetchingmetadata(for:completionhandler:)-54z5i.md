

- Link Presentation
- LPMetadataProvider
-  startFetchingMetadata(for:completionHandler:) 

Instance Method

# startFetchingMetadata(for:completionHandler:)

Fetches metadata for the given URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 18.0+visionOS 1.0+

``` source
func startFetchingMetadata(
    for URL: URL,
    completionHandler: @escaping (LPLinkMetadata?, (any Error)?) -> Void
)
```

``` source
func startFetchingMetadata(for URL: URL) async throws -> LPLinkMetadata
```

## Discussion

Call this method once per LPMetadataProvider instance. If you attempt to fetch metadata multiple times on a single LPMetadataProvider instance, it throws an error.

The completion handler executes on a background queue. Dispatch any necessary UI updates back to the main queue. When the completion handler returns, it deletes any file URLs returned in the resulting LPLinkMetadata.

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
 func startFetchingMetadata(for url: URL) async throws -> LPLinkMetadata
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Fetching metadata

func cancel()

Cancels a metadata request.

var shouldFetchSubresources: Bool

A Boolean value indicating whether to download subresources specified by the metadata.

var timeout: TimeInterval

The time interval after which the request automatically fails if it hasn’t already completed.

