

- ScreenCaptureKit
- SCScreenshotManager
-  captureImage(contentFilter:configuration:completionHandler:) 

Type Method

# captureImage(contentFilter:configuration:completionHandler:)

Captures a single frame from a stream as an image, using a filter.

Mac Catalyst 17.0+macOS 14.0+

``` source
class func captureImage(
    contentFilter: SCContentFilter,
    configuration config: SCStreamConfiguration,
    completionHandler: ((CGImage?, (any Error)?) -> Void)? = nil
)
```

``` source
class func captureImage(
    contentFilter: SCContentFilter,
    configuration config: SCStreamConfiguration
) async throws -> CGImage
```

## Parameters 

`contentFilter`  

The content filter used to select the stream.

`config`  

Configuration information for how to capture the screenshot.

`completionHandler`  

Closure that processes the screenshot taken from the streaming content.

## See Also

### Individual frame capture

class func captureSampleBuffer(contentFilter: SCContentFilter, configuration: SCStreamConfiguration, completionHandler: ((CMSampleBuffer?, (any Error)?) -> Void)?)

Captures a single frame directly from a stream’s buffer, using a filter.

