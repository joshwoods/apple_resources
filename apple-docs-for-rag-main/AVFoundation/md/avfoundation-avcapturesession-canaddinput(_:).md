

- AVFoundation
- AVCaptureSession
-  canAddInput(\_:) 

Instance Method

# canAddInput(\_:)

Determines whether you can add an input to a session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func canAddInput(_ input: AVCaptureInput) -> Bool
```

## Parameters 

`input`  

An input to add to the session.

## Return Value

true if you can add the input to the session; otherwise, false.

## Discussion

This method returns false if you can’t add an input to a capture session. This occurs, for example, if you attempt to add the input to a session twice, or if the input already belongs to another capture session.

## See Also

### Configuring Inputs

var inputs: [AVCaptureInput]

The inputs that provide media data to a capture session.

func addInput(AVCaptureInput)

Adds a capture input to the session.

func removeInput(AVCaptureInput)

Removes an input from the session.

