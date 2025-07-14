

- PHASE
-  PHASESpatialMixerDefinition 

Class

# PHASESpatialMixerDefinition

An audio-layering object that produces environmental effects and plays sound with a 3D position and orientation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESpatialMixerDefinition
```

## Mentioned in 

Playing sound from a location in a 3D scene

## Overview

This class enables the app to define a relationship between a source and listener in six degrees of freedom: orientation (roll, pitch, yaw) and a 3D position (x, y, z).

The framework plays back an audio source with *distance modeling* (see distanceModelParameters), direct path transmission effects and any combination of environmental effects, such as reverb (see PHASESpatialPipeline), and directivity (see listenerDirectivityModelParameters). 

The result enables an app to implement directive point or omnidirectional sound sources — with or without direction, respectively — and volumetric sources with a defined shape.

For a walkthrough of spatial mixing, see Playing sound from a location in a 3D scene.

## Topics

### Creating a Spatial Mixer

init(spatialPipeline: PHASESpatialPipeline)

Creates a mixer with the designated spatial pipeline.

convenience init(spatialPipeline: PHASESpatialPipeline, identifier: String)

Creates a named mixer with the designated spatial pipeline.

### Setting a Pipeline

var spatialPipeline: PHASESpatialPipeline

An object that adds sound layers for environmental effects.

### Changing Sound Over Distance

var distanceModelParameters: PHASEDistanceModelParameters?

An effect that changes sound as it carries over a distance.

### Configuring Directivity

var listenerDirectivityModelParameters: PHASEDirectivityModelParameters?

A data set that determines how well the listener hears depending on its direction relative to a sound source.

var sourceDirectivityModelParameters: PHASEDirectivityModelParameters?

A data set that directs sound such that it’s louder when directed at the listener.

## Relationships

### Inherits From

- PHASEMixerDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

