

- AVFoundation
- AVCapturePhotoOutput
-  isStillImageStabilizationScene Deprecated

Instance Property

# isStillImageStabilizationScene

A Boolean value indicating whether the scene currently being previewed by the camera warrants image stabilization.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isStillImageStabilizationScene: Bool { get }
```

## Discussion

This property’s value changes depending on the scene currently visible to the camera. For example, you might use this property to highlight controls in your app’s camera UI related to image stabilization, indicating to the user that the scene is dark enough that enabling image stabilization might be desirable.

If the photo capture output’s isStillImageStabilizationSupported value is false, this property’s value is always false.

This property supports key-value observing.

