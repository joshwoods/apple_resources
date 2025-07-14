

- RoomPlan
- RoomCaptureSession
-  isSupported 

Type Property

# isSupported

A Boolean value that indicates whether the user’s device supports the framework.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
static var isSupported: Bool { get }
```

## Discussion

Before attempting to begin a session, ensure the user’s device supports room scanning. This property is `true` if the device contains a LiDAR Scanner; otherwise, `false`.

