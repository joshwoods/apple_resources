

- PHASE
-  PHASEGroup 

Class

# PHASEGroup

A container that shares audio parameters with a collection of sounds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEGroup
```

## Overview

With all the sounds it contains, a group shares settings like gain, playback rate, mute, and solo. Groups are nonhierarchical and don’t overlap — that is, each sound event associates with only one group.

### Apply Group Settings to Sounds

You can apply settings to the sounds a group contains. For instance, an app can share volume settings with various sound effects and dialogue audio groups. The following example creates a group for background audio, such as environmental sound layers played with ambient music. By interpolating the group’s gain setting, the audio fade applies to every sound in the group.

- Swift
- Objective-C

```
// Allocate an engine and stereo mixer.
let stereoLayout = AVAudioChannelLayout(layoutTag: kAudioChannelLayoutTag_Stereo)!
let myEngine = PHASEEngine(updateMode: .automatic)
let stereoMixer = PHASEChannelMixerDefinition(channelLayout:stereoLayout)

// Create a group object.
let bgmGroup = PHASEGroup(identifier:"backgroundMusicGroup")
bgmGroup.register(engine: myEngine)

// Create a sound event node definition for background music.
let backgroundMusicSampler = PHASESamplerNodeDefinition(soundAssetIdentifier: "backgroundMusic", mixerDefinition: stereoMixer)

// Add the sound node to the group.
backgroundMusicSampler.group = myEngine.groups["backgroundMusicGroup"]

// Set group gain to zero.
bgmGroup.gain = 0

// Create a sound event to play the music.
var bgmEvent: PHASESoundEvent?
do {
    try bgmEvent = PHASESoundEvent(engine: myEngine, assetIdentifier: "backgroundMusicEventAsset")
} catch {
    fatalError("Error occurred: \(error.localizedDescription)")
}

// Queue the background music to play.
bgmEvent?.start() { reason in
    print("Started. Status: \(reason)")
}

// Fade in the music over two seconds.
bgmGroup.fadeGain(gain: 1.0, duration: 2.0, curveType: .linear)
```

```
// Create a group object.
PHASEGroup* bgmGroup = [[PHASEGroup alloc] initWithEngine:myEngine uid@"backgroundMusicGroup"];

// Create a sound event node definition for background music. 
PHASESamplerNodeDefinition* backgroundMusicSampler = [[PHASESamplerNodeDefinition alloc] initWithSoundAssetUID:@"backgroundMusic" mixerDefinition:mixer];

// Add the sound node to the group.
backgroundMusicSampler.group = myPHASEEngine.activeGroups[@"backgroundMusicGroup"];

// Set group gain to zero. 
bgmGroup.gain = 0;

// Create a sound event to play the music.
PHASESoundEvent* bgmEvent = [[PHASESoundEvent alloc] initWithEngine:_objects->mEngine
    registeredSoundEventNodeAssetUID:@"backgroundMusicEventAsset" outError:nil];

// Queue the background music to play.
NSError* myError = nil;
[bgmEvent startAndReturnError:&myError];

// Fade in the music over two seconds.
[bgmGroup fadeGain:1.0 duration:2.0 curveType:PHASECurveTypeLinear];
```

## Topics

### Creating a Group

init(identifier: String)

Creates a group with a unique name.

### Identifying the Group

var identifier: String

A unique name for the group.

### Defining the Group

func register(engine: PHASEEngine)

Adds the group to the engine’s dictionary.

func unregisterFromEngine()

Removes the group from the engine’s dictionary.

### Conrolling Loudness

var gain: Double

Modifies the volume of the group’s sounds.

func fadeGain(gain: Double, duration: Double, curveType: PHASECurveType)

Adjusts the volume of the sounds in a group gradually.

### Adjusting Playback Speed

var rate: Double

The group’s playback speed.

func fadeRate(rate: Double, duration: Double, curveType: PHASECurveType)

Adjusts the playback speed of the sounds in a group gradually.

### Silencing Sounds

func mute()

Silences the group.

func unmute()

Restores the group’s volume.

var isMuted: Bool

A Boolean value that indicates whether the app silences the group.

func solo()

Silences all other groups.

func unsolo()

Restores the other groups’ volume.

var isSoloed: Bool

A Boolean value that indicates whether the app silences all groups other than this group.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sound Grouping and Management

class PHASEGroupPreset

A collection of settings for groups.

class PHASEGroupPresetSetting

Settings for group presets.

class PHASEDucker

An object that manages competing sounds.

