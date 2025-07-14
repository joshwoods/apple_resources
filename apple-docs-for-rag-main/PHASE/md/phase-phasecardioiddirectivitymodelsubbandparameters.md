

- PHASE
-  PHASECardioidDirectivityModelSubbandParameters 

Class

# PHASECardioidDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a heart.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASECardioidDirectivityModelSubbandParameters
```

## Overview

This class defines one subband in the PHASECardioidDirectivityModelParameters class’s `subbands`. Depending on the specific shape you define with pattern and sharpness, you can attenuate sound focused at frequency to the sides of the listener, while leaving the sound in front of or behind the listener unchanged.

## Topics

### Creating Cardioid Directivity Subband Parameters

init()

Creates a data set that projects sound of a certain frequency outward in the shape of a heart.

### Sizing the Subband

var frequency: Double

A frequency in the audio spectrum where the pattern and sharpness resonate most.

### Shaping Directivity

var pattern: Double

A shape that determines the direction of sound.

var sharpness: Double

The amount that the shape overlaps with bordering subbands.

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

class PHASEConeDirectivityModelParameters

An object that directs sound in a cone-shaped curve that extends from a sound source.

class PHASEConeDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a cone.

class PHASEDirectivityModelParameters

A base class for objects that direct sound.

