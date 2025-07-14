

- PHASE
-  PHASEObject 

Class

# PHASEObject

An object in the scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEObject
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

This class models a member of your app’s scene by defining a 3D position and orientation.

The following subclasses derive from this class:

PHASESource  
An object that plays audio from a 3D location and orientation in a scene.

PHASEListener  
A central point of reference that defines the area within the scene that’s most audible to the user.

PHASEOccluder  
An object with a shape and position that blocks audio from reaching the listener.

The children array holds instances of this class to position and orient them relatively.

## Topics

### Creating an Object

init(engine: PHASEEngine)

Creates an object in the scene.

### Managing the Hierarchy

var children: [PHASEObject]

Objects that position and orient in the scene relative to the given object.

var parent: PHASEObject?

The object that this instance positions and orients relative to in the scene.

func addChild(PHASEObject) throws

Adds the given object as a child.

func removeChild(PHASEObject)

Removes the given object as a child.

func removeChildren()

Removes all child objects from the given object.

### Defining a Pose

var transform: simd_float4x4

A matrix, in local coordinates, that determines the object’s pose in the scene.

var worldTransform: simd_float4x4

A matrix, in scene coordinates, that determines the object’s pose in the scene.

### Inspecting the Orientation

class var forward: simd_float3

A vector that points forward in the local coordinate space.

class var right: simd_float3

A vector that points right in the local coordinate space.

class var up: simd_float3

A vector that points up in the local coordinate space.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PHASEListener
- PHASEOccluder
- PHASESource

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

