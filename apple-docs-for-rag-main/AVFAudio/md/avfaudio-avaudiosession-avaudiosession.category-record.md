

- AVFAudio
- AVAudioSession
- AVAudioSession.Category
-  record 

Type Property

# record

The category for recording audio while also silencing playback audio.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let record: AVAudioSession.Category
```

## Discussion

This category has the effect of silencing virtually all output on the system, for as long as the session is active. Unless you need to prevent any unexpected sounds from being played, use playAndRecord instead.

To continue recording audio when your app transitions to the background (for example, when the screen locks), add the `audio` value to the UIBackgroundModes key in your information property list file.

The user must grant permission for audio recording.

Note

Using this category doesn’t prevent phone calls, alarms, or other nonmixable audio sessions from interrupting the audio session.

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

static let soloAmbient: AVAudioSession.Category

The default audio session category.

static let audioProcessing: AVAudioSession.Category

The category for using an audio hardware codec or signal processor while not playing or recording audio.

Deprecated

