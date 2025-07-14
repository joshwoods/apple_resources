

- MediaExtension
- MERAWProcessor
-  processingParameters 

Instance Property

# processingParameters

Provides a list of processing parameters that can be changed by the client of Video Toolbox session to influence processing behavior.

macOS 15.0+

``` source
var processingParameters: [MERAWProcessingParameter] { get }
```

**Required**

## Discussion

This property value is an array of MERAWProcessingParameter objects, each describing the parameter and providing an interface where the processing parameter value may be modified.

## See Also

### Inspecting a RAW processor

var metalDeviceRegistryID: UInt64

Requests the processor use the provided Metal device for processing.

var outputColorAttachments: [String : Any]

Returns the color-related Core Video image buffer keys and values that become attachments to the output pixel buffers.

var isReadyForMoreMediaData: Bool

Indicates the readiness of the processor to accept more sample buffers.

**Required**

