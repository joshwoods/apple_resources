

- ScreenCaptureKit
- SCStreamDelegate
-  stream(\_:didStopWithError:) 

Instance Method

# stream(\_:didStopWithError:)

Tells the delegate that the stream stopped with an error.

Mac Catalyst 18.2+macOS 12.3+

``` source
optional func stream(
    _ stream: SCStream,
    didStopWithError error: any Error
)
```

## Parameters 

`stream`  

The stream that stopped.

`error`  

The error that caused the stream stoppage.

## Discussion

Note

When the `error` parameter has the code SCStreamError.Code.userStopped, the user took an intentional action to cancel the stream. Treat errors of this type as expected and recoverable failures.

