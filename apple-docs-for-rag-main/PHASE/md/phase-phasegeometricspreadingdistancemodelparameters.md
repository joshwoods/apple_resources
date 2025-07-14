

- PHASE
-  PHASEGeometricSpreadingDistanceModelParameters 

Class

# PHASEGeometricSpreadingDistanceModelParameters

An object that dissipates sound frequencies over distance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEGeometricSpreadingDistanceModelParameters
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

This class implements a *roll-off* effect — a strategy that aims to model the real-world manner in which sound changes with distance. When the distance between a sound and listener changes, the roll-off effect dissipates certain audio frequencies more than others.

### Dissipate Sound by Choosing a Roll-Off Factor

PHASE emphasizes or deemphasizes the volume loss of the mixer’s sound sources based on the rolloffFactor you choose. For example, a rolloffFactor of `1.0` reduces sound between the source and listener by 6 dB for every doubling of distance. At `2.0`, the loss doubles. At `0.5`, the loss halves.

To add a geometric-spreading distance model to a spatial sounds, set the mixer’s distanceModelParameters property to an instance of this class. For example:

- Swift
- Objective-C

```
let simpleModel = PHASEGeometricSpreadingDistanceModelParameters()
simpleModel.rolloffFactor = 1.0
spatialMixer.distanceModelParameters = simpleModel
```

```
PHASEGeometricSpreadingDistanceModelParameters* simpleModel = [[PHASEGeometricSpreadingDistanceModelParameters alloc] init];
simpleModel.rolloffFactor = 1.f;
spatialMixer.distanceModelParameters = simpleModel;
```

## Topics

### Creating the Distance Model Parameters

init()

Creates the geometric spreading distance model parameters.

### Setting the Roll-Off Factor

var rolloffFactor: Double

A value that fades specific frequencies over a distance.

## Relationships

### Inherits From

- PHASEDistanceModelParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Distance Modeling

class PHASEEnvelopeDistanceModelParameters

A graph of points and curves that shapes the volume of a sound over distance.

class PHASEDistanceModelFadeOutParameters

A distance over which the framework fades out sound.

class PHASEDistanceModelParameters

A base class for a sound’s rate of change over distance.

