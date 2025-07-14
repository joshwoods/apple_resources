

- AVFoundation
- AVAudioSessionSpatialExperience
-  bypassed 

Type Property

# bypassed

A nonspatial experience.

visionOS 1.0+

``` source
static var bypassed: AVAudioSession.BypassedSpatialExperience { get }
```

Available when `Self` is `AVAudioSession.BypassedSpatialExperience`.

## See Also

### Specifying the experience

static func fixed(soundStageSize: AVAudioSession.SoundStageSize) -> Self

Returns a fixed spatial experience configured for the specified sound stage size.

static func headTracked(soundStageSize: AVAudioSession.SoundStageSize, anchoringStrategy: AVAudioSession.AnchoringStrategy) -> Self

Returns a head-tracked spatial experience configured for the specified sound stage size and anchoring strategy.

enum SoundStageSize

Constants that specify the perceived size of sounds the audio session plays.

enum AnchoringStrategy

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

