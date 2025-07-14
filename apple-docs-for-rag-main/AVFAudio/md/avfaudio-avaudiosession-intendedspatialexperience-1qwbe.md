

- AVFAudio
- AVAudioSession
-  intendedSpatialExperience 

Instance Property

# intendedSpatialExperience

The spatial audio experience your app intends to provide the user.

visionOS 1.0+

``` source
@nonobjc
var intendedSpatialExperience: any AVAudioSessionSpatialExperience { get }
```

## See Also

### Configuring the spatial experience in visionOS

func setIntendedSpatialExperience(any AVAudioSessionSpatialExperience) throws

Sets the spatial audio experience your app intends to provide the user.

protocol AVAudioSessionSpatialExperience

A protocol that defines types of spatial audio experiences that the system supports.

struct HeadTrackedSpatialExperience

An experience where the sound a size dictated by its sound stage and location dictated by its anchoring strategy.

struct FixedSpatialExperience

An experience where the sound has a size dictated by its sound stage and is head-locked relative to the user.

struct BypassedSpatialExperience

An experience that bypasses system-provided audio spatialization.

enum AnchoringStrategy

Constants that specify how to set the origin of audio in a head-tracked spatial experience.

enum SoundStageSize

Constants that specify the perceived size of sounds the audio session plays.

var isNowPlayingCandidate: Bool

A Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

func setIsNowPlayingCandidate(Bool) throws

Sets a Boolean value that indicates whether the audio session is a candidate to be the Now Playing session.

