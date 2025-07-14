

- AVFoundation
- AVCaptureSession
-  addConnection(\_:) 

Instance Method

# addConnection(\_:)

Adds a connection to the capture session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
func addConnection(_ connection: AVCaptureConnection)
```

## Parameters 

`connection`  

The capture connection to add to the session.

## Discussion

You can only add a capture connection to a session using this method if canAddConnection(_:) returns true.

When using addInput(_:) or addOutput(_:), the session automatically forms connections between all compatible inputs and outputs. Manually adding connections is only necessary when adding an input or output with no connections.

## See Also

### Connecting Inputs and Outputs

var connections: [AVCaptureConnection]

The connections between inputs and outputs that a capture session contains.

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

