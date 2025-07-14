

- PHASE
-  PHASEOccluder 

Class

# PHASEOccluder

An object with a shape and position that blocks audio from reaching the listener.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEOccluder
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

The framework lowers the volume of an audio signal when an instance of this class positions somewhere along the path between the sound source and the listener.

For an example that demonstrates sound occlusion, see Playing sound from a location in a 3D scene.

## Topics

### Creating an Occluder

init(engine: PHASEEngine, shapes: [PHASEShape])

Creates an occluder with the given engine and shapes.

### Inspecting the Shape

var shapes: [PHASEShape]

An array of shapes that collectively define the occluder’s audio-deflecting surface and texture.

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

class PHASEListener

A central point of reference that defines the location within the scene that’s most audible to the user.

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

