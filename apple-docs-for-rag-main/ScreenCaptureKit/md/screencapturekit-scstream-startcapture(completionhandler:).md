

- ScreenCaptureKit
- SCStream
-  startCapture(completionHandler:) 

Instance Method

# startCapture(completionHandler:)

Starts the stream with a callback to indicate whether it successfully starts.

Mac Catalyst 18.2+macOS 12.3+

``` source
func startCapture(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func startCapture() async throws
```

## Parameters 

`completionHandler`  

A completion handler that provides an error if the stream fails to start.

## See Also

### Starting and stopping a stream

func stopCapture(completionHandler: (((any Error)?) -> Void)?)

Stops the stream.

