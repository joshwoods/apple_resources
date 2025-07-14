

- AVFoundation
- AVCapturePhotoOutput
-  AVCapturePhotoOutput.QualityPrioritization 

Enumeration

# AVCapturePhotoOutput.QualityPrioritization

Constants that indicate how to prioritize photo quality relative to capture speed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
enum QualityPrioritization
```

## Topics

### Specifying Priority

case speed

Speed of photo delivery is most important, even at the expense of quality.

case quality

Photo quality is most important, even at the expense of shot-to-shot time.

case balanced

Priority is balanced between photo quality and speed of delivery.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the Capture Prioritization

var maxPhotoQualityPrioritization: AVCapturePhotoOutput.QualityPrioritization

The highest quality the photo output should prepare to deliver on a capture-by-capture basis.

