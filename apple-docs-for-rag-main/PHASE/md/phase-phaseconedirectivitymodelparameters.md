

- PHASE
-  PHASEConeDirectivityModelParameters 

Class

# PHASEConeDirectivityModelParameters

An object that directs sound in a cone-shaped curve that extends from a sound source.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEConeDirectivityModelParameters
```

## Overview

This class determines that a particular frequency range in the audio spectrum emits sound in an area defined by a mathematical cone. PHASE refers to each frequency segment along the audio spectrum as a *subband*. This class contains an array of `subbands` that each direct sound in a unique cone shape. The framework outputs a blend of a frequency’s adjacent subbands for all frequencies that lie outside of those specified in the `subbands` array.

### Emit Sound in the Shape of a Cone

The following code defines a cone directivity model with two subbands. The first subband emits sound in a narrow region and the second subband outputs sound in a wider region.

- Swift
- Objective-C

```
let simpleCone = PHASEConeDirectivityModelParameters()

let coneSegment1 = PHASEConeDirectivityModelSubbandParameters()
coneSegment1.frequency = 500.0
coneSegment1.innerAngle = 60.0
coneSegment1.outerAngle = 80.0
coneSegment1.outerGain = 0.5

let coneSegment2 = PHASEConeDirectivityModelSubbandParameters()
coneSegment2.frequency = 5000.0
coneSegment2.innerAngle = 30.0
coneSegment2.outerAngle = 40.0
coneSegment2.outerGain = 0.3

simpleCone.subbands.add(coneSegment1)
simpleCone.subbands.add(coneSegment2)

spatialMixer.listenerDirectivityModelParameters = simpleCone
```

```
PHASEConeDirectivityModelParameters* simpleCone = 
    [[PHASEConeDirectivityModelParameters alloc] init];

PHASEConeDirectivityModelSubbandParameters* coneSegment1 = 
    [[PHASEConeDirectivityModelSubbandParameters alloc] init];
coneSegment1.frequency = 5000.f;
coneSegment1.innerAngle = 30.f;
coneSegment1.outerAngle = 40.f;
coneSegment1.outerGain = .3f;

PHASEConeDirectivityModelSubbandParameters* coneSegment2 = 
    [[PHASEConeDirectivityModelSubbandParameters alloc] init];
coneSegment2.frequency = 500.f;
coneSegment2.innerAngle = 60.f;
coneSegment2.outerAngle = 80.f;
coneSegment2.outerGain = .5f;

[simpleCone.subbands addObject:coneSegment1];
[simpleCone.subbands addObject:coneSegment2];

spatialMixer.listenerDirectivityModelParameters = simpleCone;
```

## Topics

### Creating the Cone Directivity Model Parameters

init(subbandParameters: [PHASEConeDirectivityModelSubbandParameters])

Creates an object that directs sound in a cone-shaped curve that extends from a sound source.

### Defining Subbands

var subbandParameters: [PHASEConeDirectivityModelSubbandParameters]

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

class PHASECardioidDirectivityModelParameters

An object that directs sound in a heart-shaped curve surrounding a sound source.

class PHASECardioidDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a heart.

class PHASEConeDirectivityModelSubbandParameters

A data set that projects sound of a certain frequency outward in the shape of a cone.

class PHASEDirectivityModelParameters

A base class for objects that direct sound.

