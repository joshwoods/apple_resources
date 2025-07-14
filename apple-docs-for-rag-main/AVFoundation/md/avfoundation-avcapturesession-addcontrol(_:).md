

- AVFoundation
- AVCaptureSession
-  addControl(\_:) 

Instance Method

# addControl(\_:)

Adds a control to a capture session.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func addControl(_ control: AVCaptureControl)
```

## Parameters 

`control`  

The capture control to add.

## Mentioned in 

Enhancing your app experience with the Camera Control

## Discussion

A capture session may not be able to add a control due to configuration reasons or limits of the host platform. Before calling this method, determine whether you can successfully add a control by calling the capture session’s canAddControl(_:) method.

You may call this method while the session is running.

Important

For a control to become active, you must set a AVCaptureSessionControlsDelegate on the session.

## See Also

### Configuring Capture Controls

var supportsControls: Bool

A Boolean value that indicates whether a capture session supports controls.

var maxControlsCount: Int

The maximum number of controls a capture session supports.

var controls: [AVCaptureControl]

The controls that allow configuring the camera system from device hardware.

func canAddControl(AVCaptureControl) -> Bool

Returns a Boolean value that indicates whether a capture session add the specified control.

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

