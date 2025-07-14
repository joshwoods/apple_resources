

- AVFoundation
- AVCaptureConnection
-  init(inputPort:videoPreviewLayer:) 

Initializer

# init(inputPort:videoPreviewLayer:)

Creates a capture connection that represents a connection between an input port and a video preview layer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
init(
    inputPort port: AVCaptureInput.Port,
    videoPreviewLayer layer: AVCaptureVideoPreviewLayer
)
```

## Parameters 

`port`  

An AVCaptureInput.Port instance that relates to an AVCaptureInput instance.

`layer`  

An AVCaptureVideoPreviewLayer instance.

## Return Value

A capture connection that represents a connection between `port` and `layer`.

## Discussion

You can add the connection this method returns to an AVCaptureSession instance with the addConnection(_:) method.

The addInput(_:): or addOutput(_:) methods automatically form connections between all compatible inputs and outputs. You don’t need to manually create and add connections to the session unless you use the primitive addInputWithNoConnections(_:) and addOutputWithNoConnections(_:) methods.

## See Also

### Creating a connection

init(inputPorts: [AVCaptureInput.Port], output: AVCaptureOutput)

Creates a capture connection that represents a connection between multiple input ports and an output.

