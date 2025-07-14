

- PHASE
-  PHASEDucker 

Class

# PHASEDucker

An object that manages competing sounds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEDucker
```

## Overview

When a sound plays in any of the source groups, this class lowers the volume of all the target groups so the listener hears the source sound more clearly. You set the source and target using PHASEGroup objects; see sourceGroups and targetGroups.

### Lower Background Music During a Monologue

When an app plays a monologue, the background music may need to lower, or *duck*, to enhance the clarity of the vocals. The following code demonstrates a ducker that configures a group for background music, and another group for the vocals.

- Swift
- Objective-C

```
let bgmGroup = PHASEGroup(identifier: "backgroundMusicGroup")
let voGroup = PHASEGroup(identifier: "voiceOverGroup")

let ducker = PHASEDucker(engine: myEngine, sourceGroups: [voGroup],
    targetGroups: [bgmGroup], gain: 0.25, attackTime: 0.25, releaseTime: 0.5,
    attackCurve: .linear, releaseCurve: .linear)

ducker.activate()
```

```
PHASEGroup* bgmGroup = [[PHASEGroup alloc] 
    initWithEngine:_objects->mEngine uid:@"backgroundMusicGroup"];
PHASEGroup* voGroup = [[PHASEGroup alloc] 
    initWithEngine:_objects->mEngine uid:@"voiceOverGroup"];

auto ducker = [[PHASEDucker alloc] 
    initWithEngine:_objects->mEngine
        sourceGroups:[NSSet setWithObject:voGroup]
        targetGroups:[NSSet setWithObject:bgmGroup]
        gain:0.25
        attackTime:0.25
        releaseTime:0.5
        attackCurve:PHASECurveTypeLinear
        releaseCurve:PHASECurveTypeLinear];

[ducker activate];
```

When an app sets up the ducking configuration in advance, PHASE automatically lowers the background music at runtime when the vocals play.

## Topics

### Creating a Ducker

init(engine: PHASEEngine, sourceGroups: Set&lt;PHASEGroup>, targetGroups: Set&lt;PHASEGroup>, gain: Double, attackTime: Double, releaseTime: Double, attackCurve: PHASECurveType, releaseCurve: PHASECurveType)

Creates an object that manages competing sounds.

### Specifying Sounds

var sourceGroups: Set&lt;PHASEGroup>

The sounds that determine volume reduction.

var targetGroups: Set&lt;PHASEGroup>

The sounds that reduce in volume.

### Configuring Volume Reduction

var gain: Double

The amount of volume reduction.

var identifier: String

A unique value for the ducker.

var isActive: Bool

A Boolean value that determines whether the ducker reduces sound.

var attackTime: Double

The amount of time for sound reduction to reach maximum strength.

var attackCurve: PHASECurveType

A mathematical curve that shapes transition progress as sound reduction begins.

var releaseTime: Double

The amount of time to transition from maximum sound reduction to no reduction.

var releaseCurve: PHASECurveType

A mathematical curve that shapes transition progress as sound reduction ends.

### Altering Sound

func activate()

Instructs the ducker to begin altering sound.

func deactivate()

Stops the ducker from altering sound.

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

class PHASEGroup

A container that shares audio parameters with a collection of sounds.

class PHASEGroupPreset

A collection of settings for groups.

class PHASEGroupPresetSetting

Settings for group presets.

