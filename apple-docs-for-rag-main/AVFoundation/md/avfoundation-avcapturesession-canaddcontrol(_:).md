

- AVFoundation
- AVCaptureSession
-  canAddControl(\_:) 

Instance Method

# canAddControl(\_:)

Returns a Boolean value that indicates whether a capture session add the specified control.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func canAddControl(_ control: AVCaptureControl) -> Bool
```

## Parameters 

`control`  

The capture control to add.

## Return Value

true if the capture session can add the control; otherwise, false.

## Mentioned in 

Enhancing your app experience with the Camera Control

## Discussion

Call this method to determine whether you can successfully add a control to a capture session using the addControl(_:) method. A capture session may not be able to add a control due to its current session configuration or if unsupported by the host platform.

## See Also

### Configuring Capture Controls

var supportsControls: Bool

A Boolean value that indicates whether a capture session supports controls.

var maxControlsCount: Int

The maximum number of controls a capture session supports.

var controls: [AVCaptureControl]

The controls that allow configuring the camera system from device hardware.

func addControl(AVCaptureControl)

Adds a control to a capture session.

func removeControl(AVCaptureControl)

Removes a control from a capture session.

func setControlsDelegate((any AVCaptureSessionControlsDelegate)?, queue: dispatch_queue_t?)

Sets a delegate object for the system to call when it activates and presents controls.

protocol AVCaptureSessionControlsDelegate

A protocol that defines the interface to respond to capture control activation and presentation events.

var controlsDelegate: (any AVCaptureSessionControlsDelegate)?

A delegate object that observes changes to the state of capture controls.

var controlsDelegateCallbackQueue: dispatch_queue_t?

The dispatch queue on which the system calls controls delegate methods.

