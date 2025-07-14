

- PHASE
-  PHASEMaterial 

Class

# PHASEMaterial

Surface characteristics that determine the acoustic properties of an object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMaterial
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

To specify the physical texture of a sound source or occluder, define the `materials` argument of the PHASEShape initializer, init(engine:mesh:materials:). The PHASEMaterialPreset contains the surface types with which you define the `preset` argument of this class’s init(engine:preset:) initializer.

## Topics

### Creating a Material

init(engine: PHASEEngine, preset: PHASEMaterialPreset)

Creates a material with the given preset.

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

enum PHASEMaterialPreset

A collection of physical surfaces that each add a unique acoustic quality to your app’s audio.

class PHASEMixerParameters

An object that specifies a mixer for sound events and orients them in 3D space.

