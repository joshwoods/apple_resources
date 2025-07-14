

- PHASE
-  PHASEListener 

Class

# PHASEListener

A central point of reference that defines the location within the scene that’s most audible to the user.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEListener
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

PHASE requires an instance of this class to play ambient or spatial audio. To output sound through an ambient mixer or spatial mixer, the app adds an instance of this class to a sound event by using PHASEMixerParameters.

For an example that demonstrates listeners, see Playing sound from a location in a 3D scene.

## Topics

### Creating a Listener

init(engine: PHASEEngine)

Creates a listener with the given engine.

### Adjusting Loudness

var gain: Double

Modifies the volume of all audio playback for the listener’s mixers.

### Instance Properties

var automaticHeadTrackingFlags: PHASEAutomaticHeadTrackingFlags

## Relationships

### Inherits From

- PHASEObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Soundscape Creation

class PHASESource

An object that plays audio from a 3D location and orientation in a scene.

class PHASEOccluder

An object with a shape and position that blocks audio from reaching the listener.

class PHASEObject

An object in the scene.

class PHASEShape

A collection of points that connect to form a 3D volume.

class Element

An object that describes the characteristics of a physical surface.

class PHASEMaterial

Surface characteristics that determine the acoustic properties of an object.

enum PHASEMaterialPreset

A collection of physical surfaces that each add a unique acoustic quality to your app’s audio.

class PHASEMixerParameters

An object that specifies a mixer for sound events and orients them in 3D space.

