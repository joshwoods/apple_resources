

- AVKit
- AVPictureInPictureControllerDelegate
-  pictureInPictureControllerWillStopPictureInPicture(\_:) 

Instance Method

# pictureInPictureControllerWillStopPictureInPicture(\_:)

Tells the delegate that Picture in Picture is about to stop.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
optional func pictureInPictureControllerWillStopPictureInPicture(_ pictureInPictureController: AVPictureInPictureController)
```

## Parameters 

`pictureInPictureController`  

The delegating controller.

## See Also

### Responding to Picture in Picture Lifecycle Events

func pictureInPictureControllerWillStartPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture is about to start.

func pictureInPictureControllerDidStartPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture started.

func pictureInPictureController(AVPictureInPictureController, failedToStartPictureInPictureWithError: any Error)

Tells the delegate that Picture in Picture failed to start.

func pictureInPictureControllerDidStopPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture stopped.

