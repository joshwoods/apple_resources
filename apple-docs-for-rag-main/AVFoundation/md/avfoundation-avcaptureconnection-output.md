

- AVFoundation
- AVCaptureConnection
-  output 

Instance Property

# output

The connection’s output port, if applicable.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
var output: AVCaptureOutput? { get }
```

## See Also

### Inspecting a connection

var inputPorts: [AVCaptureInput.Port]

An array of the connection’s input ports.

var videoPreviewLayer: AVCaptureVideoPreviewLayer?

The video preview layer associated with the connection.

var audioChannels: [AVCaptureAudioChannel]

An array of audio channels that the connection provides.

