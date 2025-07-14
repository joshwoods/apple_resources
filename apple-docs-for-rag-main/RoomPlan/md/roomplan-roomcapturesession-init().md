

- RoomPlan
- RoomCaptureSession
-  init() 

Initializer

# init()

Creates a room-capture session with the given AR session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
init()
```

## Discussion

By providing your own ARSession object, you can continue your app’s existing AR experience by seamlessly transitioning into a room-scanning session with RoomPlan. In addition, continuing an `ARSession` across multiple room-capture sessions — specifically, different rooms in the same vicinity — enables you to merge multiple CapturedRoom objects into a single captured structure. For more information, see CapturedStructure.

You can access the AR session at runtime with the arSession property.

