

- PHASE
-  PHASEMaterialPreset 

Enumeration

# PHASEMaterialPreset

A collection of physical surfaces that each add a unique acoustic quality to your app’s audio.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASEMaterialPreset
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

This enumeration defines the types of surface texture that you choose for your scene’s objects. To assign a preset to a material, define the `preset` argument for the material’s init(engine:preset:) initializer.

## Topics

### Presets

case brick

A surface characteristic that produces the acoustic quality of brick.

case cardboard

A surface characteristic that produces the acoustic quality of cardboard.

case concrete

A surface characteristic that produces the acoustic quality of concrete.

case drywall

A surface characteristic that produces the acoustic quality of drywall.

case glass

A surface characteristic that produces the acoustic quality of glass.

case wood

A surface characteristic that produces the acoustic quality of wood.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class PHASEMixerParameters

An object that specifies a mixer for sound events and orients them in 3D space.

