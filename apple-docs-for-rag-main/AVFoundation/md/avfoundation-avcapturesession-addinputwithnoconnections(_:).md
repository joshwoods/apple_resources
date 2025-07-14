

- AVFoundation
- AVCaptureSession
-  addInputWithNoConnections(\_:) 

Instance Method

# addInputWithNoConnections(\_:)

Adds a capture input to a session without forming any connections.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
func addInputWithNoConnections(_ input: AVCaptureInput)
```

## Parameters 

`input`  

The capture input to add to the session.

## Discussion

You can call this method while the session is running.

In most cases, use the addInput(_:) method to add new inputs to a session. Call this method if you require fine-grained control over which inputs connect to which outputs.

## See Also

### Connecting Inputs and Outputs

var connections: [AVCaptureConnection]

The connections between inputs and outputs that a capture session contains.

func addConnection(AVCaptureConnection)

Adds a connection to the capture session.

func canAddConnection(AVCaptureConnection) -> Bool

Determines whether a you can add a connection to a capture session.

func addOutputWithNoConnections(AVCaptureOutput)

Adds a capture output to the session without forming any connections.

func removeConnection(AVCaptureConnection)

Removes a capture connection from the session.

class AVCaptureAudioChannel

An object that monitors average and peak power levels for an audio channel in a capture connection.

