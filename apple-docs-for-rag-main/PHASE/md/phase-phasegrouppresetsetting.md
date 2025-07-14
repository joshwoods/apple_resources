

- PHASE
-  PHASEGroupPresetSetting 

Class

# PHASEGroupPresetSetting

Settings for group presets.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEGroupPresetSetting
```

## Overview

This class defines playback speed and volume rates of change that an app can apply to groups. To create a group preset setting, instantiate an object of this type and pass it to the `settings` parameter of init(engine:settings:timeToTarget:timeToReset:).

For an example of preset settings, see PHASEGroupPreset.

## Topics

### Creating a Setting

init(gain: Double, rate: Double, gainCurveType: PHASECurveType, rateCurveType: PHASECurveType)

Creates a group preset setting.

### Setting Loudness

var gain: Double

The volume of audio playback.

var gainCurveType: PHASECurveType

A rate of change for the setting’s volume.

### Setting Playback Speed

var rate: Double

The playback speed for audio.

var rateCurveType: PHASECurveType

A rate of change for the setting’s playback speed.

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

class PHASEDucker

An object that manages competing sounds.

