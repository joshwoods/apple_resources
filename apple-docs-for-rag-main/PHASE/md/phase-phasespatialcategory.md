

- PHASE
-  PHASESpatialCategory 

Structure

# PHASESpatialCategory

Sound resonance effects for spatial mixing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct PHASESpatialCategory
```

## Discussion

This class identifies the various audio layers that a spatial mixer offers as keys to the entries dictionary.

## Topics

### Creating a Spatial Category

init(rawValue: String)

Initializes a spatial category with the given string.

### Categories

static let directPathTransmission: PHASESpatialCategory

A spatial category that refers to the unfiltered audio signal.

static let earlyReflections: PHASESpatialCategory

A spatial category that refers to the earlier echoes along the duration of sound resonance.

static let lateReverb: PHASESpatialCategory

A spatial category that refers to the later echoes along the duration of sound resonance.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Sound Reflections and Resonance

class PHASESpatialPipeline

An object that specifies the volume of optional environmental effects.

class PHASESpatialPipelineEntry

An audio layer with an adjustable volume for a spatial mixer’s output.

struct Flags

Sound resonance options for a spatial pipeline.

