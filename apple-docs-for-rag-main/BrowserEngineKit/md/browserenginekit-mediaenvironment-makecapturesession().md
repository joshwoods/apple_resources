

- BrowserEngineKit
- MediaEnvironment
-  makeCaptureSession() 

Instance Method

# makeCaptureSession()

Creates a new capture session in this media environment or throws an error if it can not be created.

iOS 17.4+iPadOS 17.4+

``` source
func makeCaptureSession() throws -> AVCaptureSession
```

## Discussion

The media environment must be activated before the capture session can be started.

## See Also

### Capturing media streams

func activate() throws

Activates the media environment.

func suspend() throws

Suspends the media environment.

