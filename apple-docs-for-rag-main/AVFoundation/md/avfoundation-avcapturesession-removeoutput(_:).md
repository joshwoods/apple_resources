

- AVFoundation
- AVCaptureSession
-  removeOutput(\_:) 

Instance Method

# removeOutput(\_:)

Removes an output from a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func removeOutput(_ output: AVCaptureOutput)
```

## Parameters 

`output`  

An output to remove from the capture session.

## Discussion

You can call this method while the session is running.

## See Also

### Configuring Outputs

var outputs: [AVCaptureOutput]

The output destinations to which a captures session sends its data.

func canAddOutput(AVCaptureOutput) -> Bool

Determines whether you can add an output to a session.

func addOutput(AVCaptureOutput)

Adds an output to the capture session.

