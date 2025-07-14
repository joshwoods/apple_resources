

- PHASE
-  PHASEDistanceModelFadeOutParameters 

Class

# PHASEDistanceModelFadeOutParameters

A distance over which the framework fades out sound.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEDistanceModelFadeOutParameters
```

## Overview

For spatial sound output, the framework stops playing a sound when its distance from the listener surpases cullDistance. The framework gradually fades out the sound’s volume as the distance between the source and listener approaches cullDistance. Likewise, the framework gradually fades in the sound as the distance between the source and listener approaches `0`. A PHASEDistanceModelParameters object provides an instance of this class to a spatial mixer; for more information, see fadeOutParameters.

### Specifying a Maximum Distance That Sound Reaches

The following code demonstrates a spatial mixer’s additional fade out. By setting `fadeOutLength` to `1.0`, the framework begins to fade out a sound after its distance to the listener surpases `1.0`.

- Swift
- Objective-C

```
let fadeOut = PHASEDistanceModelFadeOutParameters(maximumDistance: 10.0,
 fadeOutLength: 1.0,
 curveType: PHASECurveType.linear)
piecewiseModel.fadeOutParameters = fadeOut
spatialMixer.distanceModelParameters = piecewiseModel
```

```
PHASEDistanceModelFadeOutParameters* fadeOut = 
    [[PHASEDistanceModelFadeOutParameters alloc] 
        initWithMaximumDistance:10.f 
        fadeOutLength:1.f curveType:PHASECurveTypeLinear];
piecewiseModel.fadeOutParameters = fadeOut;
spatialMixer.distanceModelParameters = piecewiseModel;
```

## Topics

### Creating the Distance Model Fade-Out Parameters

init(cullDistance: Double)

Creates a distance beyond which sound sources stop playing.

### Inspecting the Cull Distance

var cullDistance: Double

The distance beyond which the framework doesn’t process the sound.

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

### Distance Modeling

class PHASEGeometricSpreadingDistanceModelParameters

An object that dissipates sound frequencies over distance.

class PHASEEnvelopeDistanceModelParameters

A graph of points and curves that shapes the volume of a sound over distance.

class PHASEDistanceModelParameters

A base class for a sound’s rate of change over distance.

