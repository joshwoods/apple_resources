

- AVFoundation
- AVCaptureSession
-  removeInput(\_:) 

Instance Method

# removeInput(\_:)

Removes an input from the session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func removeInput(_ input: AVCaptureInput)
```

## Parameters 

`input`  

An input to remove from the capture session.

## Discussion

You can invoke this method while the session is running.

## See Also

### Configuring Inputs

var inputs: [AVCaptureInput]

The inputs that provide media data to a capture session.

func canAddInput(AVCaptureInput) -> Bool

Determines whether you can add an input to a session.

func addInput(AVCaptureInput)

Adds a capture input to the session.

