

- RoomPlan
- RoomCaptureSession
- RoomCaptureSession.Configuration
-  isCoachingEnabled 

Instance Property

# isCoachingEnabled

An option that indicates that the session periodically provides user instructions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
var isCoachingEnabled: Bool
```

## Discussion

When you enable this option and the framework determines the device needs a particular movement or perspective, it calls your delegate’s captureSession(_:didProvide:) and provides a particular RoomCaptureSession.Instruction that you can display to the user.

The default value is `true`.

