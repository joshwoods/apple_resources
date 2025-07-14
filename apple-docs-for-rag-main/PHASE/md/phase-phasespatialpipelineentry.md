

- PHASE
-  PHASESpatialPipelineEntry 

Class

# PHASESpatialPipelineEntry

An audio layer with an adjustable volume for a spatial mixer’s output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASESpatialPipelineEntry
```

## Overview

This property adjusts the amount of audio that passes through a spatial mixer’s pipeline (spatialPipeline) to the output. The pipeline’s entries contains an instance of this class for each type of audio layer that PHASESpatialCategory defines. Depending on the layer’s type, the audio may sound like spatial relections, environmental reverb, or the unfiltered signal. An app adjusts the layer’s presence in the mixer’s output by:

- Defining an initial volume using sendLevel

- Adjusting the audio’s volume dynamically, for example, by fading it over a duration using sendLevelMetaParameterDefinition

## Topics

### Setting the Send Level

var sendLevel: Double

The amount of audio signal to add to the output.

### Fading the Send Level

var sendLevelMetaParameterDefinition: PHASENumberMetaParameterDefinition?

A parameter that gradually updates the amount of audio signal that passes through to the output.

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

class PHASESpatialPipeline

An object that specifies the volume of optional environmental effects.

struct PHASESpatialCategory

Sound resonance effects for spatial mixing.

struct Flags

Sound resonance options for a spatial pipeline.

