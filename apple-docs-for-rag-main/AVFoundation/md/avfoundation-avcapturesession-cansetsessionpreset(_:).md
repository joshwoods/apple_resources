

- AVFoundation
- AVCaptureSession
-  canSetSessionPreset(\_:) 

Instance Method

# canSetSessionPreset(\_:)

Determines whether you can configure a capture session with the specified preset.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func canSetSessionPreset(_ preset: AVCaptureSession.Preset) -> Bool
```

## Parameters 

`preset`  

A preset value to test.

## Return Value

true if the capture session supports the preset; otherwise, false.

## Discussion

Use this method to determine whether the capture session, in its current I/O configuration, supports a particular preset. You can only set a preset that returns true as the capture session’s sessionPreset property value.

## See Also

### Setting a Session Preset

struct Preset

Presets that define standard configurations for a capture session.

var sessionPreset: AVCaptureSession.Preset

A preset value that indicates the quality level or bit rate of the output.

