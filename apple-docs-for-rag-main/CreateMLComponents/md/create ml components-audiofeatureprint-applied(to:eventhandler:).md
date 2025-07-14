

- Create ML Components
- AudioFeaturePrint
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Extracts audio features from an a sequence of audio buffers

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to input: S,
    eventHandler: EventHandler? = nil
) throws -> AudioFeaturePrint.FeatureSequence where S : TemporalSequence, S.Feature == AVAudioPCMBuffer
```

## Parameters 

`input`  

An async sequence of audio buffers.

`eventHandler`  

An event handler.

## Return Value

An async sequence of shaped arrays containing extracted features. Each shaped array has a shape of `[512]`.

## Discussion

You can call this method multiple times to process multiple streams.

## See Also

### Performing the transformation

func applied&lt;S, TS, Annotation>(to: S, eventHandler: EventHandler?) async throws -> [AnnotatedFeature&lt;Self.OutputSequence, Annotation>]

Performs the transformation on a sequence of annotated input sequences.

typealias Input

The input type.

typealias Output

The output type.

struct FeatureSequence

An async sequence of audio buffers.

