

- RoomPlan
- RoomCaptureView
-  init(frame:arSession:) 

Initializer

# init(frame:arSession:)

Creates a room-capture view with the given AR session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 16.0–1.0Deprecated

``` source
@MainActor @preconcurrency
init(
    frame: CGRect,
    arSession: ARSession
)
```

## Parameters 

`frame`  

A structure that positions and shapes the view.

`arSession`  

A world-tracking session that your app creates and runs with an ARWorldTrackingConfiguration before calling this function. If you pass an `ARSession` instance, RoomPlan preserves all of the AR session’s settings.

## Discussion

By providing your own ARSession object, you can continue your app’s existing AR experience by seamlessly transitioning into a room-scanning session wtih RoomPlan. In addition, continuing an `ARSession` across multiple room-capture sessions — specifically, different rooms in the same vicinity — enables you to merge multiple CapturedRoom objects into a single captured structure. For more information, see CapturedStructure.

You can access the `arSession` at runtime through this class’s room-capture session (captureSession) property. See the RoomCaptureSession property arSession.

## See Also

### Creating a room-capture view

init(frame: CGRect)

Creates a view that sizes to the specified frame.

init?(coder: NSCoder)

Creates a view by deserializing from the specified coder.

