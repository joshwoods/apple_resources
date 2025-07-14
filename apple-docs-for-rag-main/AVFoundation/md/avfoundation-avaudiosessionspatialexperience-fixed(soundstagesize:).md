

- AVFoundation
- AVAudioSessionSpatialExperience
-  fixed(soundStageSize:) 

Type Method

# fixed(soundStageSize:)

Returns a fixed spatial experience configured for the specified sound stage size.

visionOS 1.0+

``` source
static func fixed(soundStageSize: AVAudioSession.SoundStageSize) -> Self
```

Available when `Self` is `AVAudioSession.FixedSpatialExperience`.

## Parameters 

`soundStageSize`  

The size of the sound stage.

## Return Value

A new spatial experience.

## See Also

### Specifying the experience

static func headTracked(soundStageSize: AVAudioSession.SoundStageSize, anchoringStrategy: AVAudioSession.AnchoringStrategy) -> Self

Returns a head-tracked spatial experience configured for the specified sound stage size and anchoring strategy.

enum SoundStageSize

Constants that specify the perceived size of sounds the audio session plays.

enum AnchoringStrategy

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

static var bypassed: AVAudioSession.BypassedSpatialExperience

A nonspatial experience.

