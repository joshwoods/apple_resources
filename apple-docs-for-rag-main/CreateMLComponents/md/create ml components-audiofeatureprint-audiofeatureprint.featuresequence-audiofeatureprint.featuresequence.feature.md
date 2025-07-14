

- Create ML Components
- AudioFeaturePrint
- AudioFeaturePrint.FeatureSequence
-  AudioFeaturePrint.FeatureSequence.Feature 

Type Alias

# AudioFeaturePrint.FeatureSequence.Feature

The feature type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
typealias Feature = MLShapedArray
```

## See Also

### Creating an iterator

func makeAsyncIterator() -> AudioFeaturePrint.FeatureSequence.AsyncIterator

Constructs an iterator.

struct Iterator

An async iterator of audio buffers.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

