

- AVFoundation
- AVSampleBufferGenerator
-  notifyOfDataReady(for:completionHandler:) 

Type Method

# notifyOfDataReady(for:completionHandler:)

Notifies the sample buffer generator when data is ready for the sample buffer reference or an error has occurred.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 10.10+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
class func notifyOfDataReady(
    for sbuf: CMSampleBuffer,
    completionHandler: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
class func notifyOfDataReady(for sbuf: CMSampleBuffer) async throws
```

## Parameters 

`sbuf`  

The `CMSampleBufferRef`.

`completionHandler`  

A completion block that is called when data is ready for the sample buffer or an error occurs. The `dataReady` argument is true if data is read for the sample buffer. If an error occurs, the `error` argument contains the `NSError` object.

