

- MediaExtension
- MERAWProcessor
-  outputColorAttachments 

Instance Property

# outputColorAttachments

Returns the color-related Core Video image buffer keys and values that become attachments to the output pixel buffers.

macOS 15.0+

``` source
optional var outputColorAttachments: [String : Any] { get }
```

## Discussion

This is an optional property. Only color-related keys from Image Buffer Attachment Keys are permitted in the returned dictionary.

## See Also

### Inspecting a RAW processor

var metalDeviceRegistryID: UInt64

Requests the processor use the provided Metal device for processing.

var processingParameters: [MERAWProcessingParameter]

Provides a list of processing parameters that can be changed by the client of Video Toolbox session to influence processing behavior.

**Required**

var isReadyForMoreMediaData: Bool

Indicates the readiness of the processor to accept more sample buffers.

**Required**

