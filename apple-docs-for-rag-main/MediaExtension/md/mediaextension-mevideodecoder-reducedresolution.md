

- MediaExtension
- MEVideoDecoder
-  reducedResolution 

Instance Property

# reducedResolution

A request to decode at a lower resolution than full-size.

macOS 14.0+

``` source
optional var reducedResolution: CGSize { get set }
```

## Discussion

This optional property conveys a request for reduced resolution for decoding. Decoders that only support a fixed set of resolutions should pick the smallest resolution greater than or equal to the requested width and height. If the output CVPixelBuffer is not in a format where reduced resolution decoding is supported, this setting should be disregarded. This property is set on the extension when a Video Toolbox client sets the kVTDecompressionPropertyKey_ReducedResolutionDecode property on the hosting VTDecompressionSession.

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

var pixelFormatsWithReducedResolutionDecodeSupport: [NSNumber]

Provides a list of output pixel formats where the decoder supports reduced resolution decoding.

var producesRAWOutput: Bool

Indicates whether the decoder produces RAW output which requires the use of a RAW processor.

var isReadyForMoreMediaData: Bool

A Boolean value that indicates the readiness of the decoder to accept more sample buffers.

**Required**

