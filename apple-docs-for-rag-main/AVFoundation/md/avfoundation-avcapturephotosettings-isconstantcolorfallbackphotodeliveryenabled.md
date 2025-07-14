

- AVFoundation
- AVCapturePhotoSettings
-  isConstantColorFallbackPhotoDeliveryEnabled 

Instance Property

# isConstantColorFallbackPhotoDeliveryEnabled

A Boolean value that indicates whether to deliver a fallback photo when taking a constant color capture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isConstantColorFallbackPhotoDeliveryEnabled: Bool { get set }
```

## Discussion

The default value is false. Set the value to true to receive a fallback photo that you can use if the main constant color photo’s confidence level doesn’t meet your requirement.

## See Also

### Configuring Constant Color

var isConstantColorEnabled: Bool

A Boolean value that indicates whether to capture the photo with constant color.

