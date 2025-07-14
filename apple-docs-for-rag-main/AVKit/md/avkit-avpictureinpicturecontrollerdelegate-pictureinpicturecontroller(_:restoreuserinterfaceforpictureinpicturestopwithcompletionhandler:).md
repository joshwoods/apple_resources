

- AVKit
- AVPictureInPictureControllerDelegate
-  pictureInPictureController(\_:restoreUserInterfaceForPictureInPictureStopWithCompletionHandler:) 

Instance Method

# pictureInPictureController(\_:restoreUserInterfaceForPictureInPictureStopWithCompletionHandler:)

Tells the delegate to restore the user interface before Picture in Picture stops.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
optional func pictureInPictureController(
    _ pictureInPictureController: AVPictureInPictureController,
    restoreUserInterfaceForPictureInPictureStopWithCompletionHandler completionHandler: @escaping (Bool) -> Void
)
```

``` source
optional func pictureInPictureController(_ pictureInPictureController: AVPictureInPictureController) async -> Bool
```

## Parameters 

`pictureInPictureController`  

The delegating controller.

`completionHandler`  

You must call the completion handler with a value of true to allow the system to finish restoring your player user interface.

## Mentioned in 

Adopting Picture in Picture in a Custom Player

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func pictureInPictureController(_ pictureInPictureController: AVPictureInPictureController) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Implement this method if your player user interface requires configuration or layout to return to its default state.

