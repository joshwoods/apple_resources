

- MediaExtension
- MERAWProcessor
-  metalDeviceRegistryID 

Instance Property

# metalDeviceRegistryID

Requests the processor use the provided Metal device for processing.

macOS 15.0+

``` source
optional var metalDeviceRegistryID: UInt64 { get set }
```

## Discussion

This optional property requests that MERAWProcessor use `MTLDevice` corresponding to this ID for any Metal-based processing. This is optional and doesn’t need to be implemented if the processor does not use Metal.

## See Also

### Inspecting a RAW processor

var outputColorAttachments: [String : Any]

Returns the color-related Core Video image buffer keys and values that become attachments to the output pixel buffers.

var processingParameters: [MERAWProcessingParameter]

Provides a list of processing parameters that can be changed by the client of Video Toolbox session to influence processing behavior.

**Required**

var isReadyForMoreMediaData: Bool

Indicates the readiness of the processor to accept more sample buffers.

**Required**

