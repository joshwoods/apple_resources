

- PHASE
-  PHASEMixerParameters 

Class

# PHASEMixerParameters

An object that specifies a mixer for sound events and orients them in 3D space.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMixerParameters
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

This class orients a sound event in 3D space relative to a listener. When you configure an ambient mixer’s orientation and a listener’s orientation, PHASE lowers the volume of the sound event if the two orientations point away from each other, and plays the sound at full volume if they point at each other. To add an instance of this class to a sound event, use the `mixerParameters` argument of a sound event’s init(engine:assetIdentifier:mixerParameters:) initializer.

Alternatively, PHASE can adjust a sound event’s loudness based on its distance from the listener in 3D space. By calling this class’s addSpatialMixerParameters(identifier:source:listener:) function, you supply a sound source that defines the location. For more information, see Spatial Mixing.

Ambient sound events define only a listener and play with a consistent loudness, regardless of the listener’s position in the scene. To define a listener and select a particular ambient mixer that outputs the sound, call this class’s addAmbientMixerParameters(identifier:listener:) function.

## Topics

### Positioning and Orienting Audio

func addAmbientMixerParameters(identifier: String, listener: PHASEListener)

Adds runtime parameters for an ambient mixer.

func addSpatialMixerParameters(identifier: String, source: PHASESource, listener: PHASEListener)

Adds runtime parameters for a spatial mixer.

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

### Soundscape Creation

class PHASESource

An object that plays audio from a 3D location and orientation in a scene.

class PHASEListener

A central point of reference that defines the location within the scene that’s most audible to the user.

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

