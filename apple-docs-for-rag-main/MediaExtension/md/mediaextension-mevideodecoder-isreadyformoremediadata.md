

- MediaExtension
- MEVideoDecoder
-  isReadyForMoreMediaData 

Instance Property

# isReadyForMoreMediaData

A Boolean value that indicates the readiness of the decoder to accept more sample buffers.

macOS 14.0+

``` source
var isReadyForMoreMediaData: Bool { get }
```

**Required**

## Discussion

Video decoders which operate asynchronously often have a fixed capacity for buffers in flight in the decoder. This property allows the decoder to signal to Video Toolbox that its internal buffers are full and it can’t accept more samples. The decoder needs to use MEVideoDecoderReadyForMoreMediaDataDidChangeNotification to notify Video Toolbox when this property changes.

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

var producesRAWOutput: Bool

Indicates whether the decoder produces RAW output which requires the use of a RAW processor.

