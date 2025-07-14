

- AVFoundation
- AVCaptureSession
-  setControlsDelegate(\_:queue:) 

Instance Method

# setControlsDelegate(\_:queue:)

Sets a delegate object for the system to call when it activates and presents controls.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
func setControlsDelegate(
    _ controlsDelegate: (any AVCaptureSessionControlsDelegate)?,
    queue controlsDelegateCallbackQueue: dispatch_queue_t?
)
```

## Parameters 

`controlsDelegate`  

An object that adopts the controls delegate protocol.

`controlsDelegateCallbackQueue`  

A serial dispatch queue on which to call the delegate methods. You must specify a serial queue to ensure callbacks occur in order.

This argument must not be `nil` unless the `controlsDelegate` argument is also `nil;` otherwise, the system throws an invalidArgumentException.

## Mentioned in 

Enhancing your app experience with the Camera Control

## Discussion

People interact with capture controls by performing specific gestures to enable their visibility. Specify a delegate to for the system to call when it presents and dismisses controls. The system calls the delegate’s methods on the specified callback queue.

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

func addControl(AVCaptureControl)

Adds a control to a capture session.

func removeControl(AVCaptureControl)

Removes a control from a capture session.

protocol AVCaptureSessionControlsDelegate

A protocol that defines the interface to respond to capture control activation and presentation events.

var controlsDelegate: (any AVCaptureSessionControlsDelegate)?

A delegate object that observes changes to the state of capture controls.

var controlsDelegateCallbackQueue: dispatch_queue_t?

The dispatch queue on which the system calls controls delegate methods.

