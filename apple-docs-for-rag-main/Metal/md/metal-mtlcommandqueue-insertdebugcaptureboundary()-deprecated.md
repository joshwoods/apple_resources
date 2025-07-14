

- Metal
- MTLCommandQueue
-  insertDebugCaptureBoundary() Deprecated

Instance Method

# insertDebugCaptureBoundary()

Informs Xcode about when GPU Frame Capture starts and stops.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.13DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
func insertDebugCaptureBoundary()
```

**Required**

Deprecated

Use MTLCaptureManager and MTLCaptureScope instead. See `Enhancing Frame Capture by Using Labels` for more information.

## Discussion

You can explicitly define the boundary between two GPU captures by calling this method, which overrides Xcode’s default behavior when you enable GPU Frame Capture. If your app doesn’t call the method, Xcode adds a frame boundary each time your app calls the present(_:) or present(_:atTime:) methods.

For example, an app with a single drawable may not need this method because the default behavior’s implicit frame boundaries are appropriate for that scenario.

However, you may want to create explicit frame boundaries for apps with multiple drawables that produce frames at different rates.

In this example scenario, the app uses three drawables, each of which presents their frames at different rates or times. The developer can use this method to add arbitrary boundaries that create two captures. The first capture contains the first two frames from Drawable A, the first frame from Drawable B, and the first frame from Drawable C. The second capture contains the third and fourth frames from Drawable A, the second frame from Drawable B, and the second and third frames from Drawable C.

Warning

Don’t call this method from within the completion handler you pass to addCompletedHandler(_:) because it can trigger a deadlock when you capture a GPU frame.

