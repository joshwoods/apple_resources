

- Link Presentation
- LPLinkMetadata
-  remoteVideoURL 

Instance Property

# remoteVideoURL

A remote URL corresponding to a representative video for the URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var remoteVideoURL: URL? { get set }
```

## Discussion

This may reference a remote video file that AVFoundation can stream, or a YouTube video URL.

## See Also

### Getting the link’s video

var videoProvider: NSItemProvider?

An object that retrieves data corresponding to a representative video for the URL.

