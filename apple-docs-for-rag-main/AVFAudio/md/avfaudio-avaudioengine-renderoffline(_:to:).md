

- AVFAudio
- AVAudioEngine
-  renderOffline(\_:to:) 

Instance Method

# renderOffline(\_:to:)

Makes a render call to the engine operating in the offline manual rendering mode.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func renderOffline(
    _ numberOfFrames: AVAudioFrameCount,
    to buffer: AVAudioPCMBuffer
) throws -> AVAudioEngineManualRenderingStatus
```

## Parameters 

`numberOfFrames`  

The number of PCM sample frames to render.

`buffer`  

The PCM buffer the engine must render the audio for.

## Return Value

One of the status codes from AVAudioEngineManualRenderingStatus. Irrespective of the returned status code, on exit, the output buffer’s frameLength indicates the number of PCM samples the engine renders.

## See Also

### Manually Rendering an Audio Engine

func enableManualRenderingMode(AVAudioEngineManualRenderingMode, format: AVAudioFormat, maximumFrameCount: AVAudioFrameCount) throws

Sets the engine to operate in manual rendering mode with the render format and maximum frame count you specify.

func disableManualRenderingMode()

Sets the engine to render to or from an audio device.

