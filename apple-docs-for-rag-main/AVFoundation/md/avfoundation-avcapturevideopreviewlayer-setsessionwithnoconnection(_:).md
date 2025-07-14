

- AVFoundation
- AVCaptureVideoPreviewLayer
-  setSessionWithNoConnection(\_:) 

Instance Method

# setSessionWithNoConnection(\_:)

Associates a session with the layer without automatically forming a connection to an eligible input port.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func setSessionWithNoConnection(_ session: AVCaptureSession)
```

## Parameters 

`session`  

A capture session.

## Discussion

Only use this method if you intend to manually create a connection between the layer and a particular AVCaptureInput.Port, and add it to the session using its addConnection(_:) method.

## See Also

### Session Configuration

var session: AVCaptureSession?

A capture session with visual output to preview.

var connection: AVCaptureConnection?

An object that describes the connection from the layer to a particular input port.

