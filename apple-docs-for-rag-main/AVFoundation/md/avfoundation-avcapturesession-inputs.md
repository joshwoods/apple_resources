

- AVFoundation
- AVCaptureSession
-  inputs 

Instance Property

# inputs

The inputs that provide media data to a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var inputs: [AVCaptureInput] { get }
```

## Discussion

You add new inputs to a capture session by callings its addInput(_:) method.

## See Also

### Configuring Inputs

func canAddInput(AVCaptureInput) -> Bool

Determines whether you can add an input to a session.

func addInput(AVCaptureInput)

Adds a capture input to the session.

func removeInput(AVCaptureInput)

Removes an input from the session.

