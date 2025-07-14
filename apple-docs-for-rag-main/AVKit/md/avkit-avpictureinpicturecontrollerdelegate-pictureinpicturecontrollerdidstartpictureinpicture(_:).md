

- AVKit
- AVPictureInPictureControllerDelegate
-  pictureInPictureControllerDidStartPictureInPicture(\_:) 

Instance Method

# pictureInPictureControllerDidStartPictureInPicture(\_:)

Tells the delegate that Picture in Picture started.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
optional func pictureInPictureControllerDidStartPictureInPicture(_ pictureInPictureController: AVPictureInPictureController)
```

## Parameters 

`pictureInPictureController`  

The delegating controller.

## See Also

### Responding to Picture in Picture Lifecycle Events

func pictureInPictureControllerWillStartPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture is about to start.

func pictureInPictureController(AVPictureInPictureController, failedToStartPictureInPictureWithError: any Error)

Tells the delegate that Picture in Picture failed to start.

func pictureInPictureControllerWillStopPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture is about to stop.

func pictureInPictureControllerDidStopPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture stopped.

