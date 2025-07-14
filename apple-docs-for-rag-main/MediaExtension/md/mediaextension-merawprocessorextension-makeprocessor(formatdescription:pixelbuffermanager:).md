

- MediaExtension
- MERAWProcessorExtension
-  makeProcessor(formatDescription:pixelBufferManager:) 

Instance Method

# makeProcessor(formatDescription:pixelBufferManager:)

A factory method to create a video RAW processor.

macOS 15.0+

``` source
func makeProcessor(
    formatDescription: CMVideoFormatDescription,
    pixelBufferManager extensionPixelBufferManager: MERAWProcessorPixelBufferManager
) throws -> any MERAWProcessor
```

**Required**

## Parameters 

`formatDescription`  

A `CMVideoFormatDescription` describing the video data that was decoded to produce the RAW input for the video RAW processor.

`extensionPixelBufferManager`  

An `MERAWProcessorPixelBufferManager` instance that should be retained by the new `MERAWProcessor` instance and used for output pixelBuffer configuration and allocation.

## Discussion

Creates a new `MERAWProcessor` matching the given `CMVideoFormatDescriptionRef`. If these parameters are not compatible with the `MERAWProcessor`, the call should fail, returning `MEErrorUnsupportedFeature`.

