

- PHASE
-  PHASESource 

Class

# PHASESource

An object that plays audio from a 3D location and orientation in a scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESource
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

This class represents a sound-emitting point or area in a virtual environment, positioned and oriented by a 3D transform.

A spatial mixer, PHASESpatialMixerDefinition, adds environmental effects to sound sources. To tie a mixer to a sound source, create a PHASEMixerParameters object and pass it into the `mixerParameters` argument of a sound event’s init(engine:assetIdentifier:mixerParameters:) initializer.

For an example that demonstrates sound sources, see Playing sound from a location in a 3D scene.

## Topics

### Creating a Source

init(engine: PHASEEngine)

Creates a single point in the environment from which sound emanates.

init(engine: PHASEEngine, shapes: [PHASEShape])

Creates a voluminous area in the environment from which sound emanates.

### Controlling Sound Volume

var gain: Double

The amount of sound the source emanates.

### Inspecting the Shape

var shapes: [PHASEShape]

An array of shapes that collectively define the audio-emitting surface area of a volumetric source.

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

class PHASEMixerParameters

An object that specifies a mixer for sound events and orients them in 3D space.

