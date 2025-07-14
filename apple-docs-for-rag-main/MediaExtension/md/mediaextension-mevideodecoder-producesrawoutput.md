

- MediaExtension
- MEVideoDecoder
-  producesRAWOutput 

Instance Property

# producesRAWOutput

Indicates whether the decoder produces RAW output which requires the use of a RAW processor.

macOS 14.0+

``` source
optional var producesRAWOutput: Bool { get }
```

## Discussion

The extension should implement this property returning YES if the decoder produces RAW output which requires the use of an MERAWProcessor for post-decode processing to produce renderable output.

This optional property is queried on the extension when a Video Toolbox client queries the kVTDecompressionPropertyKey_DecoderProducesRAWOutput property on the hosting VTDecompressionSession.

## See Also

### Inspecting a video decoder

var contentHasInterframeDependencies: Bool

A Boolean that specifies whether the content has interframe dependencies, if the decoder knows.

var recommendedThreadCount: Int

The recommended number of threads for the decoder to use.

var actualThreadCount: Int

The actual number of threads the decoder uses.

var supportedPixelFormatsOrderedByQuality: [NSNumber]

Provides hints about quality tradeoffs between pixel formats.

var reducedResolution: CGSize

A request to decode at a lower resolution than full-size.

var pixelFormatsWithReducedResolutionDecodeSupport: [NSNumber]

Provides a list of output pixel formats where the decoder supports reduced resolution decoding.

var isReadyForMoreMediaData: Bool

A Boolean value that indicates the readiness of the decoder to accept more sample buffers.

**Required**

