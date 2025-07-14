

- AVFoundation
- AVCapturePhotoOutput
-  maxPhotoQualityPrioritization 

Instance Property

# maxPhotoQualityPrioritization

The highest quality the photo output should prepare to deliver on a capture-by-capture basis.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
var maxPhotoQualityPrioritization: AVCapturePhotoOutput.QualityPrioritization { get set }
```

## Discussion

AVCapturePhotoOutput can apply a variety of techniques to improve photo quality, such as reducing noise, preserving detail in low light, freezing motion, and so on. Some techniques improve image quality at the expense of the shot-to-shot time. Before starting your session, you may set this property to indicate the highest quality prioritization you intend to request when calling the capturePhoto(with:delegate:) method.

When configuring an AVCapturePhotoSettings object, you can’t exceed this quality prioritization level, but you may select a lower prioritization level that favors speed over quality.

When you attach the photo output to an AVCaptureSession, the default value of this property is AVCapturePhotoOutput.QualityPrioritization.balanced. If you instead attach it to an AVCaptureMultiCamSession, the default value is AVCapturePhotoOutput.QualityPrioritization.speed.

Important

Changing the value of this property while the session is running causes the session to be rebuilt. This can be an expensive operation that will interrupt video preview until complete.

## See Also

### Setting the Capture Prioritization

enum QualityPrioritization

Constants that indicate how to prioritize photo quality relative to capture speed.

