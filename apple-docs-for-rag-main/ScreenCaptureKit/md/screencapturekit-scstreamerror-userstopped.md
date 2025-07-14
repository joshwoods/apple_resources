

- ScreenCaptureKit
- SCStreamError
-  userStopped 

Type Property

# userStopped

An error message that indicates the user stopped the stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
static var userStopped: SCStreamError.Code { get }
```

## Discussion

As a best practice, handle errors of this type as an intentional user interaction rather than an error.

