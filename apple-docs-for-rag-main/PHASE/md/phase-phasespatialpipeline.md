

- PHASE
-  PHASESpatialPipeline 

Class

# PHASESpatialPipeline

An object that specifies the volume of optional environmental effects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESpatialPipeline
```

## Overview

The PHASESpatialMixerDefinition class contains an instance of this class, spatialPipeline, to add optional sound layers to the output.

On top of the original audio signal designated by directPathTransmission, this class optionally includes audio layers for environmental effects, such as earlyReflections or lateReverb, in the output. To control the amount of volume that either audio layer possesses in the mixer’s output, adjust the sendLevel for the layer’s respective PHASESpatialPipelineEntry member in the entries dictionary.

## Topics

### Creating a Spatial Pipeline

init?(flags: PHASESpatialPipeline.Flags)

Creates a spatial pipeline with the specified flags.

struct Flags

Sound resonance options for a spatial pipeline.

### Inspecting Effects

var flags: PHASESpatialPipeline.Flags

A collection of environmental effects to include in the output.

var entries: [PHASESpatialCategory : PHASESpatialPipelineEntry]

Audio layers for environmental effects to add to the output.

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

### Sound Reflections and Resonance

class PHASESpatialPipelineEntry

An audio layer with an adjustable volume for a spatial mixer’s output.

struct PHASESpatialCategory

Sound resonance effects for spatial mixing.

struct Flags

Sound resonance options for a spatial pipeline.

