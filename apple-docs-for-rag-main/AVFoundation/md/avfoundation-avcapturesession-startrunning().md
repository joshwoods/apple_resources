

- AVFoundation
- AVCaptureSession
-  startRunning() 

Instance Method

# startRunning()

Starts the flow of data through the capture pipeline.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func startRunning()
```

## Mentioned in 

Setting Up a Capture Session

## Discussion

Call this method to start the flow of data from the capture session’s inputs to its outputs. This method is synchronous and blocks until the session starts running or it fails, which it reports by posting an runtimeErrorNotification notification.

## See Also

### Managing the Session Life Cycle

func stopRunning()

Stops the flow of data through the capture pipeline.

