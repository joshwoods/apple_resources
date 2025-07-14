

- AVFoundation
- AVCaptureConnection
-  init(inputPorts:output:) 

Initializer

# init(inputPorts:output:)

Creates a capture connection that represents a connection between multiple input ports and an output.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
init(
    inputPorts ports: [AVCaptureInput.Port],
    output: AVCaptureOutput
)
```

## Parameters 

`ports`  

An array of AVCaptureInput.Port instances that relate to AVCaptureInput instances.

`output`  

An AVCaptureOutput instance.

## Return Value

A capture connection that represents a connection between `ports` and `output`.

## Discussion

You can add the connection this method returns to an AVCaptureSession instance with the addConnection(_:) method.

The addInput(_:): or addOutput(_:) methods automatically form connections between all compatible inputs and outputs. You don’t need to manually create and add connections to the session unless you use the primitive addInputWithNoConnections(_:) and addOutputWithNoConnections(_:) methods.

## See Also

### Creating a connection

init(inputPort: AVCaptureInput.Port, videoPreviewLayer: AVCaptureVideoPreviewLayer)

Creates a capture connection that represents a connection between an input port and a video preview layer.

