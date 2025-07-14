

- AVFoundation
- AVCaptureConnection
-  audioChannels 

Instance Property

# audioChannels

An array of audio channels that the connection provides.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var audioChannels: [AVCaptureAudioChannel] { get }
```

## Discussion

The property only applies to a video connection.

## See Also

### Inspecting a connection

var inputPorts: [AVCaptureInput.Port]

An array of the connection’s input ports.

var output: AVCaptureOutput?

The connection’s output port, if applicable.

var videoPreviewLayer: AVCaptureVideoPreviewLayer?

The video preview layer associated with the connection.

