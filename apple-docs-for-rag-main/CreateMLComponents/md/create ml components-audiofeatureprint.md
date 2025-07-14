

- Create ML Components
-  AudioFeaturePrint 

Structure

# AudioFeaturePrint

A stream transformer that extracts audio features from audio buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct AudioFeaturePrint
```

## Topics

### Creating a transformer

init(windowDuration: TimeInterval, overlapFactor: Double)

Creates an audio feature print feature extractor.

### Getting the properties

let overlapFactor: Double

The overlap factor of the extractor.

let windowDuration: TimeInterval

The window duration of the extractor.

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) throws -> AudioFeaturePrint.FeatureSequence

Extracts audio features from an a sequence of audio buffers

func applied&lt;S, TS, Annotation>(to: S, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;Self.OutputSequence, Annotation>]

Performs the transformation on a sequence of annotated input sequences.

typealias Input

The input type.

typealias Output

The output type.

struct FeatureSequence

An async sequence of audio buffers.

### Type Aliases

typealias OutputSequence

The output async sequence type.

### Default Implementations

CustomDebugStringConvertible Implementations

TemporalTransformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Sendable
- TemporalTransformer

## See Also

### Audio components

struct AudioReader

An audio file reader.

struct AudioConvertingTransformer

A transformer for audio conversion.

