

- AVFoundation
- AVCaptureConnection
-  inputPorts 

Instance Property

# inputPorts

An array of the connection’s input ports.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
var inputPorts: [AVCaptureInput.Port] { get }
```

## Discussion

Input ports are instances of AVCaptureInput.Port.

## See Also

### Inspecting a connection

var output: AVCaptureOutput?

The connection’s output port, if applicable.

var videoPreviewLayer: AVCaptureVideoPreviewLayer?

The video preview layer associated with the connection.

var audioChannels: [AVCaptureAudioChannel]

An array of audio channels that the connection provides.

