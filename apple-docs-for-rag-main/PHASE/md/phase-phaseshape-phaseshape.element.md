

- PHASE
- PHASEShape
-  PHASEShape.Element 

Class

# PHASEShape.Element

An object that describes the characteristics of a physical surface.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class Element
```

## Overview

This class defines the material that makes up a PHASEShape object.

You don’t instantiate instances of this class yourself; the framework creates an instance of this class for every material you pass into the init(engine:mesh:materials:) initializer. The shape’s elements array provides read-only access to the instances.

## Topics

### Specifying a Meterial

var material: PHASEMaterial?

A surface characteristic that determines the acoustic properties of an object.

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

class PHASEMaterial

Surface characteristics that determine the acoustic properties of an object.

enum PHASEMaterialPreset

A collection of physical surfaces that each add a unique acoustic quality to your app’s audio.

class PHASEMixerParameters

An object that specifies a mixer for sound events and orients them in 3D space.

