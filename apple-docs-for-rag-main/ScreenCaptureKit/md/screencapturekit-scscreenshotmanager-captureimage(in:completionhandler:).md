

- ScreenCaptureKit
- SCScreenshotManager
-  captureImage(in:completionHandler:) 

Type Method

# captureImage(in:completionHandler:)

Mac Catalyst 18.2+macOS 15.2+

``` source
class func captureImage(
    in rect: CGRect,
    completionHandler: ((CGImage?, (any Error)?) -> Void)? = nil
)
```

``` source
class func captureImage(in rect: CGRect) async throws -> CGImage
```

