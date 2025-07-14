

- AVFoundation
- AVCaptureConnection
-  videoPreviewLayer 

Instance Property

# videoPreviewLayer

The video preview layer associated with the connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var videoPreviewLayer: AVCaptureVideoPreviewLayer? { get }
```

## Discussion

The connection sets the property in its init(inputPort:videoPreviewLayer:) initializer.

## See Also

### Inspecting a connection

var inputPorts: [AVCaptureInput.Port]

An array of the connection’s input ports.

var output: AVCaptureOutput?

The connection’s output port, if applicable.

var audioChannels: [AVCaptureAudioChannel]

An array of audio channels that the connection provides.

