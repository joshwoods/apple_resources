

- AVKit
- AVPictureInPictureControllerDelegate
-  pictureInPictureController(\_:failedToStartPictureInPictureWithError:) 

Instance Method

# pictureInPictureController(\_:failedToStartPictureInPictureWithError:)

Tells the delegate that Picture in Picture failed to start.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
optional func pictureInPictureController(
    _ pictureInPictureController: AVPictureInPictureController,
    failedToStartPictureInPictureWithError error: any Error
)
```

## Parameters 

`pictureInPictureController`  

The delegating controller.

`error`  

An error that describes the details of the failure.

## See Also

### Responding to Picture in Picture Lifecycle Events

func pictureInPictureControllerWillStartPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture is about to start.

func pictureInPictureControllerDidStartPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture started.

func pictureInPictureControllerWillStopPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture is about to stop.

func pictureInPictureControllerDidStopPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture stopped.

