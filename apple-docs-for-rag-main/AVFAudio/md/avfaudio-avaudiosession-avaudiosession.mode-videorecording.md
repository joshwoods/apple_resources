

- AVFAudio
- AVAudioSession
- AVAudioSession.Mode
-  videoRecording 

Type Property

# videoRecording

A mode that indicates that your app is recording a movie.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let videoRecording: AVAudioSession.Mode
```

## Discussion

This mode is valid only with the record and playAndRecord audio session categories. On devices with more than one built-in microphone, the audio session uses the microphone closest to the video camera.

Use this mode to ensure that the system provides appropriate audio-signal processing.

Use AVCaptureSession in conjunction with the video recording mode for greater control of input and output routes. For example, setting the automaticallyConfiguresApplicationAudioSession property results in the session automatically choosing the best input route for the device and camera used.

## See Also

### Getting Standard Session Modes

static let `default`: AVAudioSession.Mode

The default audio session mode.

static let gameChat: AVAudioSession.Mode

A mode that the GameKit framework sets on behalf of an application that uses GameKit’s voice chat service.

static let measurement: AVAudioSession.Mode

A mode that indicates that your app is performing measurement of audio input or output.

static let moviePlayback: AVAudioSession.Mode

A mode that indicates that your app is playing back movie content.

static let spokenAudio: AVAudioSession.Mode

A mode used for continuous spoken audio to pause the audio when another app plays a short audio prompt.

static let videoChat: AVAudioSession.Mode

A mode that indicates that your app is engaging in online video conferencing.

static let voiceChat: AVAudioSession.Mode

A mode that indicates that your app is performing two-way voice communication, such as using Voice over Internet Protocol (VoIP).

static let voicePrompt: AVAudioSession.Mode

A mode that indicates that your app plays audio using text-to-speech.

