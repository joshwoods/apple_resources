

- Link Presentation
-  LPMetadataProvider 

Class

# LPMetadataProvider

An object that retrieves metadata for a URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 18.0+visionOS 1.0+

``` source
class LPMetadataProvider
```

## Overview

Use LPMetadataProvider to fetch metadata for a URL, including its title, icon, and image or video links. All properties on the resulting LPLinkMetadata instance are optional.

Note

To enable macOS clients to fetch metadata for remote URLs, add the com.apple.security.network.client entitlement.

## Fetch link metadata from a URL

For each metadata request, create an instance of LPMetadataProvider and call startFetchingMetadata(for:completionHandler:).

In the completion handler, check the error. If your user doesn’t have a network connection, the fetch can fail. If the server doesn’t respond or is too slow, the fetch can time out. Alternatively, the app may cancel the request, or an unknown error may occur.

Otherwise, use the metadata however you want, for example, to populate the title for a table view cell.

```
let metadataProvider = LPMetadataProvider()
let url = URL(string: "https://www.apple.com/ipad")!

metadataProvider.startFetchingMetadata(for: url) { metadata, error in
    if error != nil {
        // The fetch failed; handle the error.
        return
    }

    // Make use of fetched metadata.
}
```

For more information about handling errors, see LPError.

## Topics

### Fetching metadata

func startFetchingMetadata(for: URL, completionHandler: (LPLinkMetadata?, (any Error)?) -> Void)

Fetches metadata for the given URL.

func cancel()

Cancels a metadata request.

var shouldFetchSubresources: Bool

A Boolean value indicating whether to download subresources specified by the metadata.

var timeout: TimeInterval

The time interval after which the request automatically fails if it hasn’t already completed.

### Instance Methods

func startFetchingMetadata(for: URLRequest, completionHandler: (LPLinkMetadata?, (any Error)?) -> Void)

Fetches metadata for the given `NSURLRequest`.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Link metadata

class LPLinkMetadata

An object that contains metadata about a URL.

