

- AVFoundation
- AVCaptureSession
-  addInput(\_:) 

Instance Method

# addInput(\_:)

Adds a capture input to the session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func addInput(_ input: AVCaptureInput)
```

## Parameters 

`input`  

An input to add to the session.

## Discussion

It’s only valid to call this method if canAddInput(_:) returns true.

You can invoke this method while the session is running.

## See Also

### Configuring Inputs

var inputs: [AVCaptureInput]

The inputs that provide media data to a capture session.

func canAddInput(AVCaptureInput) -> Bool

Determines whether you can add an input to a session.

func removeInput(AVCaptureInput)

Removes an input from the session.

