

- ScreenCaptureKit
- SCStreamError
- SCStreamError.Code
-  SCStreamError.Code.userStopped 

Case

# SCStreamError.Code.userStopped

An error message that indicates the user stopped the stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
case userStopped
```

## Discussion

As a best practice, handle errors of this type as an intentional user interaction rather than an error.

