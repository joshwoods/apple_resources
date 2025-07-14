

- AVKit
-  AVPictureInPictureControllerDelegate 

Protocol

# AVPictureInPictureControllerDelegate

A protocol to adopt to respond to Picture in Picture events.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
protocol AVPictureInPictureControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Adopting Picture in Picture in a Custom Player

Adopting Picture in Picture for video calls

## Overview

Adopt this protocol in a custom object, and assign the object as the delegate of your AVPictureInPictureController instance.

## Topics

### Restoring the User Interface

func pictureInPictureController(AVPictureInPictureController, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the user interface before Picture in Picture stops.

### Responding to Picture in Picture Lifecycle Events

func pictureInPictureControllerWillStartPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture is about to start.

func pictureInPictureControllerDidStartPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture started.

func pictureInPictureController(AVPictureInPictureController, failedToStartPictureInPictureWithError: any Error)

Tells the delegate that Picture in Picture failed to start.

func pictureInPictureControllerWillStopPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture is about to stop.

func pictureInPictureControllerDidStopPictureInPicture(AVPictureInPictureController)

Tells the delegate that Picture in Picture stopped.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Accessing the Delegate Object

var delegate: (any AVPictureInPictureControllerDelegate)?

A delegate object for a Picture in Picture controller.

