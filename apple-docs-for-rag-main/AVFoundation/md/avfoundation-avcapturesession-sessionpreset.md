

- AVFoundation
- AVCaptureSession
-  sessionPreset 

Instance Property

# sessionPreset

A preset value that indicates the quality level or bit rate of the output.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var sessionPreset: AVCaptureSession.Preset { get set }
```

## Discussion

Specify a preset value to configure a capture session’s format and settings. The default preset is high, which produces high-quality video and audio output, but you can specify any preset value that returns true for a call to canSetSessionPreset(_:).

You can set this value while the session is running.

## See Also

### Setting a Session Preset

struct Preset

Presets that define standard configurations for a capture session.

func canSetSessionPreset(AVCaptureSession.Preset) -> Bool

Determines whether you can configure a capture session with the specified preset.

