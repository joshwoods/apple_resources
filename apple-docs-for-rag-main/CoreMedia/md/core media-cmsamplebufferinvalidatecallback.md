

- Core Media
-  CMSampleBufferInvalidateCallback 

Type Alias

# CMSampleBufferInvalidateCallback

Client callback called by CMSampleBufferInvalidate(_:).

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMSampleBufferInvalidateCallback = (CMSampleBuffer, UInt64) -> Void
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being invalidated.

`invalidateRefCon`  

Reference constant provided when the callback was set up.

