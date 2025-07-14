

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
- AVCaptureDevice.Format.AutoFocusSystem
-  AVCaptureDevice.Format.AutoFocusSystem.phaseDetection 

Case

# AVCaptureDevice.Format.AutoFocusSystem.phaseDetection

A faster autofoscus system based on differences in light phase.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
case phaseDetection
```

## Discussion

Phase detection has the ability to achieve focus in many cases without a focus scan. Phase detection autofocus is typically less visually intrusive than contrast detection autofocus.

## See Also

### Systems

case none

Autofocus isn’t available.

case contrastDetection

A slower autofocus system based on differences in contrast.

