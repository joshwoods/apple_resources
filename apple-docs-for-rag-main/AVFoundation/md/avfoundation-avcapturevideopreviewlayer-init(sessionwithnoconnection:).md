

- AVFoundation
- AVCaptureVideoPreviewLayer
-  init(sessionWithNoConnection:) 

Initializer

# init(sessionWithNoConnection:)

Creates a layer to preview the visual output of a capture session, without making connections to eligible video inputs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
init(sessionWithNoConnection session: AVCaptureSession)
```

## Parameters 

`session`  

A capture session to preview.

## Discussion

Only use this initializer if you intend to manually connect the layer to a particular AVCaptureInput.Port by calling the session’s addConnection(_:) method.

## See Also

### Creating a Preview Layer

init(session: AVCaptureSession)

Creates a layer to preview the visual output of a capture session.

