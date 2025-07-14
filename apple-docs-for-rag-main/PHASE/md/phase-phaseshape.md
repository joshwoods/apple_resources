

- PHASE
-  PHASEShape 

Class

# PHASEShape

A collection of points that connect to form a 3D volume.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEShape
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

To define your scene’s important 3D volumes, create one or more of the following surfaces and add them to your scene’s shapes array:

- The audio-emitting surface of a volumetric PHASESource

- The audio-deflecting surface and texture of a PHASEOccluder

## Topics

### Creating a Shape

init(engine: PHASEEngine, mesh: MDLMesh)

Creates an object that the given geometric data shapes.

convenience init(engine: PHASEEngine, mesh: MDLMesh, materials: [PHASEMaterial])

Creates an object of a specific material that the given geometric data shapes.

### Describing Surface Characteristics

var elements: [PHASEShape.Element]

An array of objects that collectively describe the physical characteristics of a surface.

class Element

An object that describes the characteristics of a physical surface.

## Relationships

### Inherits From

- NSObject

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

class PHASEOccluder

An object with a shape and position that blocks audio from reaching the listener.

class PHASEObject

An object in the scene.

class Element

An object that describes the characteristics of a physical surface.

class PHASEMaterial

Surface characteristics that determine the acoustic properties of an object.

enum PHASEMaterialPreset

A collection of physical surfaces that each add a unique acoustic quality to your app’s audio.

class PHASEMixerParameters

An object that specifies a mixer for sound events and orients them in 3D space.

