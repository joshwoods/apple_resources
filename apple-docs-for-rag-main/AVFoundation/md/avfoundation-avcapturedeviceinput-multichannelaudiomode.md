

- AVFoundation
- AVCaptureDeviceInput
-  multichannelAudioMode 

Instance Property

# multichannelAudioMode

The multichannel audio mode to apply when recording audio.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var multichannelAudioMode: AVCaptureMultichannelAudioMode { get set }
```

## Discussion

This property only takes effect when the system routes audio through the built-in microphone. The system ignores the value when an external microphone is in use.

The default value is AVCaptureMultichannelAudioMode.none, which indicates to use single channel audio recording.

## See Also

### Configuring audio properties

func isMultichannelAudioModeSupported(AVCaptureMultichannelAudioMode) -> Bool

A Boolean value that indicates whether the input supports the specified multichannel audio mode.

enum AVCaptureMultichannelAudioMode

Constants that indicate the modes of multichannel audio.

