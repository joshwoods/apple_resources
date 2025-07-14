

- PHASE
-  PHASECardioidDirectivityModelParameters 

Class

# PHASECardioidDirectivityModelParameters

An object that directs sound in a heart-shaped curve surrounding a sound source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASECardioidDirectivityModelParameters
```

## Overview

This class configures a particular frequency range in the audio spectrum that emits sound in an area defined by a mathematical cardioid. PHASE refers to each frequency segment along the audio spectrum as a *subband*. This class contains an array of `subbands` that each can direct sound in a unique cardioid shape. The framework outputs a blend of a frequency’s adjacent subbands for all frequencies that lie outside of those specified in the `subbands` array.

### Emit Sound in the Shape of a Cardioid

The following code defines a two-band cardioid model. The first subband resembles a heart-shaped cardioid and the second resembles a hypercardioid.

- Swift
- Objective-C

```
let simpleCardioid = PHASECardioidDirectivityModelParameters()

// Create a cardioid model.
var cardioidSegment1 = PHASECardioidDirectivityModelSubbandParameters()
cardioidSegment1.frequency = 500.0
cardioidSegment1.pattern = 0.5 // Cardioid shape
cardioidSegment1.sharpness = 1.0

// Create a hypercardioid model.
var cardioidSegment2 = PHASECardioidDirectivityModelSubbandParameters()
cardioidSegment2.frequency = 5000.0
cardioidSegment2.pattern = 0.75
cardioidSegment2.sharpness = 1.5

simpleCardioid.subbands.add(cardioidSegment1)
simpleCardioid.subbands.add(cardioidSegment2)

spatialMixer.sourceDirectivityModelParameters = simpleCardioid
```

```
PHASECardioidDirectivityModelParameters* simpleCardioid = [[PHASECardioidDirectivityModelParameters alloc] init];

// Create a cardioid model.
PHASECardioidDirectivityModelSubbandParameters* cardioidSegment1 = [[PHASECardioidDirectivityModelSubbandParameters alloc] init];
cardioidSegment1.frequency = 500.f;
cardioidSegment1.pattern = .5f; 
cardioidSegment1.sharpness = 1.f;

// Create a hypercardioid model.
PHASECardioidDirectivityModelSubbandParameters* cardioidSegment2 = [[PHASECardioidDirectivityModelSubbandParameters alloc] init];
cardioidSegment2.frequency = 5000.f;
cardioidSegment2.pattern = .75f;
cardioidSegment2.sharpness = 1.5f;

[simpleCardioid.subbands addObject:cardioidSegment1];
[simpleCardioid.subbands addObject:cardioidSegment2];

spatialMixer.sourceDirectivityModelParameters = simpleCardioid;
```

## Topics

### Creating the Cardioid Directivity Model Parameters

init(subbandParameters: [PHASECardioidDirectivityModelSubbandParameters])

Creates an object that directs sound in a heart-shaped curve surrounding a sound source.

### Defining Subbands

var subbandParameters: [PHASECardioidDirectivityModelSubbandParameters]

An array of frequencies that describe varying sound emission across the spectrum.

## Relationships

### Inherits From

- PHASEDirectivityModelParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sound Directivity

class PHASECardioidDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a heart.

class PHASEConeDirectivityModelParameters

An object that directs sound in a cone-shaped curve that extends from a sound source.

class PHASEConeDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a cone.

class PHASEDirectivityModelParameters

A base class for objects that direct sound.

