

- ScreenCaptureKit
- SCScreenshotManager
-  captureSampleBuffer(contentFilter:configuration:completionHandler:) 

Type Method

# captureSampleBuffer(contentFilter:configuration:completionHandler:)

Captures a single frame directly from a stream’s buffer, using a filter.

Mac Catalyst 17.0+macOS 14.0+

``` source
class func captureSampleBuffer(
    contentFilter: SCContentFilter,
    configuration config: SCStreamConfiguration,
    completionHandler: ((CMSampleBuffer?, (any Error)?) -> Void)? = nil
)
```

``` source
class func captureSampleBuffer(
    contentFilter: SCContentFilter,
    configuration config: SCStreamConfiguration
) async throws -> CMSampleBuffer
```

## Parameters 

`contentFilter`  

The content filter used to select the stream.

`config`  

Configuration information for how to record the stream buffer.

`completionHandler`  

Closure that processes the capture taken from streaming content.

## See Also

### Individual frame capture

class func captureImage(contentFilter: SCContentFilter, configuration: SCStreamConfiguration, completionHandler: ((CGImage?, (any Error)?) -> Void)?)

Captures a single frame from a stream as an image, using a filter.

