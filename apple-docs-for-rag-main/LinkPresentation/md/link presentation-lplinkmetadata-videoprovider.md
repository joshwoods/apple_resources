

- Link Presentation
- LPLinkMetadata
-  videoProvider 

Instance Property

# videoProvider

An object that retrieves data corresponding to a representative video for the URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var videoProvider: NSItemProvider? { get set }
```

## Discussion

The item provider returns a video that AVFoundation can play.

## See Also

### Getting the link’s video

var remoteVideoURL: URL?

A remote URL corresponding to a representative video for the URL.

