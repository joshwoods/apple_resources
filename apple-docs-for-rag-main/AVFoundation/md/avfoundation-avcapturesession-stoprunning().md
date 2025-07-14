

- AVFoundation
- AVCaptureSession
-  stopRunning() 

Instance Method

# stopRunning()

Stops the flow of data through the capture pipeline.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func stopRunning()
```

## Discussion

Call this method to stop the flow of data from the inputs to the outputs connected to the capture session. This method is synchronous and blocks until the session stops running completely.

## See Also

### Managing the Session Life Cycle

func startRunning()

Starts the flow of data through the capture pipeline.

