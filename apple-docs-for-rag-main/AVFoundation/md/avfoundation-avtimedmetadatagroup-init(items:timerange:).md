

- AVFoundation
- AVTimedMetadataGroup
-  init(items:timeRange:) 

Initializer

# init(items:timeRange:)

Creates a timed metadata group initialized with the given metadata items.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(
    items: [AVMetadataItem],
    timeRange: CMTimeRange
)
```

## Parameters 

`items`  

An array of AVMetadataItem objects.

`timeRange`  

The time range of the metadata contained in `items`.

## Return Value

A metadata group initialized with `items`.

## See Also

### Creating a Timed Metadata Group

init?(sampleBuffer: CMSampleBuffer)

Creates a timed metadata group with a sample buffer.

