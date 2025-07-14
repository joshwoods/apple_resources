

- AVFoundation
- AVCaptureVideoPreviewLayer
-  connection 

Instance Property

# connection

An object that describes the connection from the layer to a particular input port.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var connection: AVCaptureConnection? { get }
```

## Mentioned in 

Setting Up a Capture Session

## Discussion

When you associate a preview layer with a capture session, the session automatically creates a connection to the first eligible video AVCaptureInput.Port object. If you detach a preview layer from a session, the connection property becomes `nil`.

## See Also

### Session Configuration

var session: AVCaptureSession?

A capture session with visual output to preview.

func setSessionWithNoConnection(AVCaptureSession)

Associates a session with the layer without automatically forming a connection to an eligible input port.

