

- MediaExtension
- MEVideoDecoder
-  supportedPixelFormatsOrderedByQuality 

Instance Property

# supportedPixelFormatsOrderedByQuality

Provides hints about quality tradeoffs between pixel formats.

macOS 14.0+

``` source
optional var supportedPixelFormatsOrderedByQuality: [NSNumber] { get }
```

## Discussion

This array contains CMPixelFormatType values, ordered by quality from best to worst. The system queries this property on the extension when Video Toolbox queries the kVTDecompressionPropertyKey_SupportedPixelFormatsOrderedByQuality on the hosting VTDecompressionSession.

## See Also

### Inspecting a video decoder

var contentHasInterframeDependencies: Bool

A Boolean that specifies whether the content has interframe dependencies, if the decoder knows.

var recommendedThreadCount: Int

The recommended number of threads for the decoder to use.

var actualThreadCount: Int

The actual number of threads the decoder uses.

var reducedResolution: CGSize

A request to decode at a lower resolution than full-size.

var pixelFormatsWithReducedResolutionDecodeSupport: [NSNumber]

Provides a list of output pixel formats where the decoder supports reduced resolution decoding.

var producesRAWOutput: Bool

Indicates whether the decoder produces RAW output which requires the use of a RAW processor.

var isReadyForMoreMediaData: Bool

A Boolean value that indicates the readiness of the decoder to accept more sample buffers.

**Required**

