

- Video Toolbox
- VTFrameProcessorConfiguration
-  minimumDimensions 

Type Property

# minimumDimensions

The minimum dimensions of a source frame for the processor.

macOS 15.4+

``` source
optional static var minimumDimensions: CMVideoDimensions { get }
```

## See Also

### Inspecting the required configuration

var frameSupportedPixelFormats: [NSNumber]

A list of supported pixel formats for the current configuration.

**Required**

var sourcePixelBufferAttributes: [AnyHashable : Any]

A dictionary of pixel buffer attributes that define what the source and reference frames passed to the processor must conform to.

**Required**

var destinationPixelBufferAttributes: [AnyHashable : Any]

A dictionary of pixel buffer attributes that define which output frames passed to the processor must conform to.

**Required**

var nextFrameCount: Int

The number of next frames that the processor requires for processing.

var previousFrameCount: Int

The number of previous frames that the processor requires for processing.

static var maximumDimensions: CMVideoDimensions

The maximum dimensions of a source frame for the processor.

