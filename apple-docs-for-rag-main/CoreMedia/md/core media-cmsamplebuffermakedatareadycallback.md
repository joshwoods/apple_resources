

- Core Media
-  CMSampleBufferMakeDataReadyCallback 

Type Alias

# CMSampleBufferMakeDataReadyCallback

Client callback called by CMSampleBufferMakeDataReady(_:).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMSampleBufferMakeDataReadyCallback = (CMSampleBuffer, UnsafeMutableRawPointer?) -> OSStatus
```

## Parameters 

`sbuf`  

The sample buffer to make ready.

`makeDataReadyRefcon`  

Client refcon provided to `CMSampleBufferCreate`.

For example, it could point at info about the scheduled read that needs to be forced to finish.

## Discussion

This callback must make the data ready (e.g. force a scheduled read to finish). If this callback succeeds and returns 0, the sample buffer will then be marked as “data ready”.

