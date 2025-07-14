

- AVKit
- AVPictureInPictureController
-  contentSource 

Instance Property

# contentSource

The source of the controller’s content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var contentSource: AVPictureInPictureController.ContentSource? { get set }
```

## Discussion

You can change a content source while a Picture in Picture session is active, but only if the new content source is ready for display. If it isn’t ready, the session ends immediately.

If your app uses AVPlayerLayer, verify that the value of its isReadyForDisplay property is true before setting it as a content source.

## See Also

### Configuring the Content Source

class ContentSource

An object that represents the source of the content to present in Picture in Picture.

