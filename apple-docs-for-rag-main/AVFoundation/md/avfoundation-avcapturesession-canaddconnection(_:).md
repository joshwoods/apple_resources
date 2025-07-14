

- AVFoundation
- AVCaptureSession
-  canAddConnection(\_:) 

Instance Method

# canAddConnection(\_:)

Determines whether a you can add a connection to a capture session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
func canAddConnection(_ connection: AVCaptureConnection) -> Bool
```

## Parameters 

`connection`  

A connect object to test.

## Return Value

true if you can add the connection; otherwise, false.

## See Also

### Connecting Inputs and Outputs

var connections: [AVCaptureConnection]

The connections between inputs and outputs that a capture session contains.

func addConnection(AVCaptureConnection)

Adds a connection to the capture session.

func addInputWithNoConnections(AVCaptureInput)

Adds a capture input to a session without forming any connections.

func addOutputWithNoConnections(AVCaptureOutput)

Adds a capture output to the session without forming any connections.

func removeConnection(AVCaptureConnection)

Removes a capture connection from the session.

class AVCaptureAudioChannel

An object that monitors average and peak power levels for an audio channel in a capture connection.

