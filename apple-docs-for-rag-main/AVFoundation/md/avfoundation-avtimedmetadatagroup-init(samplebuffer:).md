

- AVFoundation
- AVTimedMetadataGroup
-  init(sampleBuffer:) 

Initializer

# init(sampleBuffer:)

Creates a timed metadata group with a sample buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init?(sampleBuffer: CMSampleBuffer)
```

## Parameters 

`sampleBuffer`  

A CMSampleBuffer with media type kCMMediaType_Metadata.

## Return Value

An instance of `AVTimedMetadataGroup`.

## See Also

### Creating a Timed Metadata Group

init(items: [AVMetadataItem], timeRange: CMTimeRange)

Creates a timed metadata group initialized with the given metadata items.

