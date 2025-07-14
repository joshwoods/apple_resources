

- MediaExtension
- MERAWProcessor
-  isReadyForMoreMediaData 

Instance Property

# isReadyForMoreMediaData

Indicates the readiness of the processor to accept more sample buffers.

macOS 15.0+

``` source
var isReadyForMoreMediaData: Bool { get }
```

**Required**

## Discussion

An MERAWProcessor operates asynchronously and often has a fixed capacity for buffers in flight in the processor. This property allows the processor to signal to Video Toolbox that its internal buffers are full and cannot accept more samples. The processor must use MERAWProcessorReadyForMoreMediaDataDidChangeNotification to notify Video Toolbox when this property changes.

## See Also

### Inspecting a RAW processor

var metalDeviceRegistryID: UInt64

Requests the processor use the provided Metal device for processing.

var outputColorAttachments: [String : Any]

Returns the color-related Core Video image buffer keys and values that become attachments to the output pixel buffers.

var processingParameters: [MERAWProcessingParameter]

Provides a list of processing parameters that can be changed by the client of Video Toolbox session to influence processing behavior.

**Required**

