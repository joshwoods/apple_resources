

- AVFAudio
- AVAudioSession
- AVAudioSession.Category
-  audioProcessing Deprecated

Type Property

# audioProcessing

The category for using an audio hardware codec or signal processor while not playing or recording audio.

iOS 3.0–10.0DeprecatediPadOS 3.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let audioProcessing: AVAudioSession.Category
```

Deprecated

This category is no longer necessary and was deprecated iOS 10.

## Discussion

This category disables playback (audio output) and disables recording (audio input). Use this category, for example, when performing offline audio format conversion.

## See Also

### Getting Standard Categories

static let ambient: AVAudioSession.Category

The category for an app in which sound playback is nonprimary — that is, your app also works with the sound turned off.

static let multiRoute: AVAudioSession.Category

The category for routing distinct streams of audio data to different output devices at the same time.

static let playAndRecord: AVAudioSession.Category

The category for recording (input) and playback (output) of audio, such as for a Voice over Internet Protocol (VoIP) app.

static let playback: AVAudioSession.Category

The category for playing recorded music or other sounds that are central to the successful use of your app.

static let record: AVAudioSession.Category

The category for recording audio while also silencing playback audio.

static let soloAmbient: AVAudioSession.Category

The default audio session category.

