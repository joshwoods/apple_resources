

- AVKit
- AVPictureInPictureController
-  init(contentSource:) 

Initializer

# init(contentSource:)

Creates a Picture in Picture controller with a content source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(contentSource: AVPictureInPictureController.ContentSource)
```

## Parameters 

`contentSource`  

The source of the content to show in a Picture in Picture window.

## Discussion

Use this initializer to create a controller that displays its content in a player layer or a sample buffer display layer.

Important

Before attempting to create a controller, verify that the current device supports Picture in Picture by calling the isPictureInPictureSupported() class method. Attempting to create a Picture in Picture controller on an unsupported device returns `nil`.

## See Also

### Creating a Controller

convenience init?(playerLayer: AVPlayerLayer)

Creates a Picture in Picture controller with a player layer.

