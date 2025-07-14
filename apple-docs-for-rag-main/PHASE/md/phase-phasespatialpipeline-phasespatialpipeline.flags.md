

- PHASE
- PHASESpatialPipeline
-  PHASESpatialPipeline.Flags 

Structure

# PHASESpatialPipeline.Flags

Sound resonance options for a spatial pipeline.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Flags
```

## Overview

Each PHASESpatialPipeline specifies a flag in its init(flags:) initializer.

## Topics

### Creating a Flag

init(rawValue: UInt)

Initializes a spatial flag with the given string.

### Choosing a Flag

static var directPathTransmission: PHASESpatialPipeline.Flags

A spatial property that refers to the original audio signal.

static var earlyReflections: PHASESpatialPipeline.Flags

A spatial property that refers to the earlier echoes along the duration of sound resonance.

static var lateReverb: PHASESpatialPipeline.Flags

A spatial property that refers to the later echoes along the duration of sound resonance.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Sound Reflections and Resonance

class PHASESpatialPipeline

An object that specifies the volume of optional environmental effects.

class PHASESpatialPipelineEntry

An audio layer with an adjustable volume for a spatial mixer’s output.

struct PHASESpatialCategory

Sound resonance effects for spatial mixing.

