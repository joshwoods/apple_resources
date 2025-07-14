

- AVFoundation
- AVCaptureDeviceInput
-  isMultichannelAudioModeSupported(\_:) 

Instance Method

# isMultichannelAudioModeSupported(\_:)

A Boolean value that indicates whether the input supports the specified multichannel audio mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func isMultichannelAudioModeSupported(_ multichannelAudioMode: AVCaptureMultichannelAudioMode) -> Bool
```

## Parameters 

`multichannelAudioMode`  

The multichannel audio mode to test.

## Return Value

true if the input supports the mode; otherwise, false.

## Discussion

You can only set the multichannelAudioMode property if the input supports the value.

Note

Multichannel audio modes aren’t supported when used in with AVCaptureMultiCamSession.

## See Also

### Configuring audio properties

var multichannelAudioMode: AVCaptureMultichannelAudioMode

The multichannel audio mode to apply when recording audio.

enum AVCaptureMultichannelAudioMode

Constants that indicate the modes of multichannel audio.

