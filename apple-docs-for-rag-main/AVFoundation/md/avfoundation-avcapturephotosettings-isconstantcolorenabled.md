

- AVFoundation
- AVCapturePhotoSettings
-  isConstantColorEnabled 

Instance Property

# isConstantColorEnabled

A Boolean value that indicates whether to capture the photo with constant color.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isConstantColorEnabled: Bool { get set }
```

## Discussion

The default value is false. Set the value to true to capture a constant color photo.

Important

Attempting to enable constant color capture when a photo output’s isConstantColorEnabled is false, results in the system throwing an exception.

## See Also

### Configuring Constant Color

var isConstantColorFallbackPhotoDeliveryEnabled: Bool

A Boolean value that indicates whether to deliver a fallback photo when taking a constant color capture.

