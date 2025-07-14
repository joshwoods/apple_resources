

- PHASE
-  PHASEConeDirectivityModelSubbandParameters 

Class

# PHASEConeDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a cone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEConeDirectivityModelSubbandParameters
```

## Overview

This class defines one subband in the PHASEConeDirectivityModelParameters class’s `subbands`. The inner and outer angles you define with setAngles(innerAngle:outerAngle:) describe a cone that directs sound of a given frequency toward the listener. The cone’s point rests at the 3D position of the sound source. The framework adjusts the volume of the sound according to location of the listener in the 3D scene:

- If the listener positions in an area outside of the subband’s outerAngle, the sound emanates from the source at the volume defined by outerGain.

- If the listener positions inside the area defined by innerAngle, the sound emanates from the source at maximum volume.

- If the listener positions in between the outer and inner angles, the framework blends the volume to a value between outerGain and the maximum.

## Topics

### Creating Cone Directivity Subband Parameters

init()

Creates a data set that projects sound of a certain frequency outward in the shape of a cone.

### Sizing the Subband

var frequency: Double

A frequency in the audio spectrum where the subband resonates most.

### Shaping Directivity

var innerAngle: Double

An angle, in degrees, that determines the size of the audio emitting area inside the cone.

var outerAngle: Double

An angle, in degrees, that determines the size of the audio emitting area outside the cone.

var outerGain: Double

The loudness of the audio the outside area of the cone emits.

func setAngles(innerAngle: Double, outerAngle: Double)

Configures a focus area for cone-based sound directivity.

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

### Sound Directivity

class PHASECardioidDirectivityModelParameters

An object that directs sound in a heart-shaped curve surrounding a sound source.

class PHASECardioidDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a heart.

class PHASEConeDirectivityModelParameters

An object that directs sound in a cone-shaped curve that extends from a sound source.

class PHASEDirectivityModelParameters

A base class for objects that direct sound.

