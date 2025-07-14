

- Core Media
-  CMSampleBufferInvalidateHandler 

Type Alias

# CMSampleBufferInvalidateHandler

Client callback called by CMSampleBufferInvalidate(_:).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMSampleBufferInvalidateHandler = (CMSampleBuffer) -> Void
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being invalidated.

