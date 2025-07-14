

- AVFoundation
- AVCaptureSession
-  outputs 

Instance Property

# outputs

The output destinations to which a captures session sends its data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var outputs: [AVCaptureOutput] { get }
```

## Discussion

You add new outputs to a capture session by calling its addOutput(_:) method.

## See Also

### Configuring Outputs

func canAddOutput(AVCaptureOutput) -> Bool

Determines whether you can add an output to a session.

func addOutput(AVCaptureOutput)

Adds an output to the capture session.

func removeOutput(AVCaptureOutput)

Removes an output from a capture session.

