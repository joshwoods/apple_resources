

- Link Presentation
- LPMetadataProvider
-  startFetchingMetadata(for:completionHandler:) 

Instance Method

# startFetchingMetadata(for:completionHandler:)

Fetches metadata for the given `NSURLRequest`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func startFetchingMetadata(
    for request: URLRequest,
    completionHandler: @escaping (LPLinkMetadata?, (any Error)?) -> Void
)
```

``` source
func startFetchingMetadata(for request: URLRequest) async throws -> LPLinkMetadata
```

## Discussion

Call this method once per LPMetadataProvider instance. If you attempt to fetch metadata multiple times on a single LPMetadataProvider instance, it throws an error.

The completion handler executes on a background queue. Dispatch any necessary UI updates back to the main queue. When the completion handler returns, it deletes any file URLs returned in the resulting LPLinkMetadata.

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
 func startFetchingMetadata(for request: URLRequest) async throws -> LPLinkMetadata
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

