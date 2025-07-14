

- AVFoundation
- AVCaptureVideoPreviewLayer
-  session 

Instance Property

# session

A capture session with visual output to preview.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var session: AVCaptureSession? { get set }
```

## Mentioned in 

Setting Up a Capture Session

## See Also

### Session Configuration

var connection: AVCaptureConnection?

An object that describes the connection from the layer to a particular input port.

func setSessionWithNoConnection(AVCaptureSession)

Associates a session with the layer without automatically forming a connection to an eligible input port.

