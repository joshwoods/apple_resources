

- UIKit
- UIApplication
-  userDidTakeScreenshotNotification 

Type Property

# userDidTakeScreenshotNotification

A notification that posts when a person takes a screenshot on the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
class let userDidTakeScreenshotNotification: NSNotification.Name
```

## Discussion

This notification doesn’t contain a `userInfo` dictionary. This notification posts after the screenshot is taken.

