

- ScreenCaptureKit
- SCStream
-  stopCapture(completionHandler:) 

Instance Method

# stopCapture(completionHandler:)

Stops the stream.

Mac Catalyst 18.2+macOS 12.3+

``` source
func stopCapture(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func stopCapture() async throws
```

## Parameters 

`completionHandler`  

A completion handler that provides an error if the stream fails to stop.

## See Also

### Starting and stopping a stream

func startCapture(completionHandler: (((any Error)?) -> Void)?)

Starts the stream with a callback to indicate whether it successfully starts.

