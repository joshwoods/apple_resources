

- AVFoundation
- AVCaptureSession
-  addOutput(\_:) 

Instance Method

# addOutput(\_:)

Adds an output to the capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func addOutput(_ output: AVCaptureOutput)
```

## Parameters 

`output`  

An output to add to the session.

## Discussion

You can only add an output to a session using this method if canAddOutput(_:) returns true.

You can invoke this method while the session is running.

## See Also

### Configuring Outputs

var outputs: [AVCaptureOutput]

The output destinations to which a captures session sends its data.

func canAddOutput(AVCaptureOutput) -> Bool

Determines whether you can add an output to a session.

func removeOutput(AVCaptureOutput)

Removes an output from a capture session.

