

- AVFAudio
- AVAudioSession
- AVAudioSession.Category
-  playAndRecord 

Type Property

# playAndRecord

The category for recording (input) and playback (output) of audio, such as for a Voice over Internet Protocol (VoIP) app.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let playAndRecord: AVAudioSession.Category
```

## Discussion

Your audio continues with the Silent switch set to silent and with the screen locked. (The switch is called the *Ring/Silent switch* on iPhone.) To continue playing audio when your app transitions to the background (for example, when the screen locks), add the `audio` value to the UIBackgroundModes key in your information property list file.

This category is appropriate for simultaneous recording and playback, and also for apps that record and play back, but not simultaneously.

By default, using this category implies that your app’s audio is nonmixable—activating your session will interrupt any other audio sessions which are also nonmixable. To allow mixing for this category, use the mixWithOthers option.

The user must grant permission for audio recording.

This category supports the mirrored version of Airplay. However, AirPlay mirroring will be disabled if the `AVAudioSessionModeVoiceChat` mode is used with this category.

## See Also

### Getting Standard Categories

static let ambient: AVAudioSession.Category

The category for an app in which sound playback is nonprimary — that is, your app also works with the sound turned off.

static let multiRoute: AVAudioSession.Category

The category for routing distinct streams of audio data to different output devices at the same time.

static let playback: AVAudioSession.Category

The category for playing recorded music or other sounds that are central to the successful use of your app.

static let record: AVAudioSession.Category

The category for recording audio while also silencing playback audio.

static let soloAmbient: AVAudioSession.Category

The default audio session category.

static let audioProcessing: AVAudioSession.Category

The category for using an audio hardware codec or signal processor while not playing or recording audio.

Deprecated

