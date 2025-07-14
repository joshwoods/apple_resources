

- Create ML Components
- AudioFeaturePrint
-  AudioFeaturePrint.Input 

Type Alias

# AudioFeaturePrint.Input

The input type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias Input = AVAudioPCMBuffer
```

## See Also

### Performing the transformation

func applied&lt;S>(to: S, eventHandler: EventHandler?) throws -> AudioFeaturePrint.FeatureSequence

Extracts audio features from an a sequence of audio buffers

func applied&lt;S, TS, Annotation>(to: S, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;Self.OutputSequence, Annotation>]

Performs the transformation on a sequence of annotated input sequences.

typealias Output

The output type.

struct FeatureSequence

An async sequence of audio buffers.

