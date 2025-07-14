

- AVFoundation
- AVCaptureSession
-  removeConnection(\_:) 

Instance Method

# removeConnection(\_:)

Removes a capture connection from the session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
func removeConnection(_ connection: AVCaptureConnection)
```

## Parameters 

`connection`  

The capture connection to remove from the session.

## Discussion

You can call this method while the session is running.

## See Also

### Connecting Inputs and Outputs

var connections: [AVCaptureConnection]

The connections between inputs and outputs that a capture session contains.

func addConnection(AVCaptureConnection)

Adds a connection to the capture session.

func canAddConnection(AVCaptureConnection) -> Bool

Determines whether a you can add a connection to a capture session.

func addInputWithNoConnections(AVCaptureInput)

Adds a capture input to a session without forming any connections.

func addOutputWithNoConnections(AVCaptureOutput)

Adds a capture output to the session without forming any connections.

class AVCaptureAudioChannel

An object that monitors average and peak power levels for an audio channel in a capture connection.

