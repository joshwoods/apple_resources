

- AVFAudio
- AVAudioSession
-  AVAudioSession.Category 

Structure

# AVAudioSession.Category

Audio session category identifiers.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct Category
```

## Discussion

An audio session category defines a set of audio behaviors. Choose a category that most accurately describes the audio behavior you require.

### Supporting AirPlay

The playback-only categories (ambient, soloAmbient, and playback) support both the mirrored and nonmirrored variants of AirPlay.

The audio session category playAndRecord supports only the mirrored variant of AirPlay, while the record and multiRoute categories don’t allow routing to AirPlay.

Important

SharePlay and the Group Activities API only support audio sessions using the playback category. Attempting to activate a session that uses an unsupported category results in an error.

## Topics

### Creating a Category

init(rawValue: String)

Creates a new instance with the raw value you specify.

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

static let audioProcessing: AVAudioSession.Category

The category for using an audio hardware codec or signal processor while not playing or recording audio.

Deprecated

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the category configuration

var category: AVAudioSession.Category

The current audio session category.

var availableCategories: [AVAudioSession.Category]

The audio session categories available on the current device.

var categoryOptions: AVAudioSession.CategoryOptions

The set of options associated with the current audio session category.

struct CategoryOptions

Constants that specify optional audio behaviors.

