

- PHASE
-  PHASEDistanceModelParameters 

Class

# PHASEDistanceModelParameters

A base class for a sound’s rate of change over distance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEDistanceModelParameters
```

## Overview

When your app outputs sound with a 3D position and orientation, designate a subclass of this class to indicate the manner in which PHASE changes sound with distance. Assign an instance of either PHASEGeometricSpreadingDistanceModelParameters or PHASEEnvelopeDistanceModelParameters, depending on your app’s needs, to the PHASESpatialMixerDefinition class’s distanceModelParameters property.

## Topics

### Fading the Sound

var fadeOutParameters: PHASEDistanceModelFadeOutParameters?

A distance over which the framework fades out the mixer’s sound.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PHASEEnvelopeDistanceModelParameters
- PHASEGeometricSpreadingDistanceModelParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Distance Modeling

class PHASEGeometricSpreadingDistanceModelParameters

An object that dissipates sound frequencies over distance.

class PHASEEnvelopeDistanceModelParameters

A graph of points and curves that shapes the volume of a sound over distance.

class PHASEDistanceModelFadeOutParameters

A distance over which the framework fades out sound.

