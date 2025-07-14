

- Core Media
- CMSampleBuffer
- CMSampleBuffer.DataReadiness
-  CMSampleBuffer.DataReadiness.failed(\_:) 

Case

# CMSampleBuffer.DataReadiness.failed(\_:)

The system failed to load the media data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case failed(OSStatus)
```

## Parameters 

`status`  

An `OSStatus` value that indicates the cause of the failure.

## See Also

### States

case notReady

The media data isn’t ready to use.

case ready

The media data is ready to use.

