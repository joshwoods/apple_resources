

- AVFoundation
- AVCaptureSession
-  connections 

Instance Property

# connections

The connections between inputs and outputs that a capture session contains.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 1.0+

``` source
var connections: [AVCaptureConnection] { get }
```

## Discussion

A capture session automatically forms connections between inputs and outputs when you call the addInput(_:) or addOutput(_:) methods. You can explicitly add connections to a session by calling the addConnection(_:) method.

## See Also

### Connecting Inputs and Outputs

func addConnection(AVCaptureConnection)

Adds a connection to the capture session.

func canAddConnection(AVCaptureConnection) -> Bool

Determines whether a you can add a connection to a capture session.

func addInputWithNoConnections(AVCaptureInput)

Adds a capture input to a session without forming any connections.

func addOutputWithNoConnections(AVCaptureOutput)

Adds a capture output to the session without forming any connections.

func removeConnection(AVCaptureConnection)

Removes a capture connection from the session.

class AVCaptureAudioChannel

An object that monitors average and peak power levels for an audio channel in a capture connection.

