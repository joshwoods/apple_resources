

- Link Presentation
- LPLinkMetadata
-  url 

Instance Property

# url

The URL that returned the metadata, taking server-side redirects into account.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var url: URL? { get set }
```

## Discussion

The URL that returns the metadata may differ from the originalURL to which you sent the metadata request. This can happen if the server redirects the request, for example, when a resource has moved, or when the original URL is a domain alias.

## See Also

### Identifying the link

var originalURL: URL?

The original URL of the metadata request.

