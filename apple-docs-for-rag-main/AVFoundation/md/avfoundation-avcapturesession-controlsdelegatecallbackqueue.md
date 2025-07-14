

- AVFoundation
- AVCaptureSession
-  controlsDelegateCallbackQueue 

Instance Property

# controlsDelegateCallbackQueue

The dispatch queue on which the system calls controls delegate methods.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var controlsDelegateCallbackQueue: dispatch_queue_t? { get }
```

## Discussion

Call the setControlsDelegate(_:queue:) method to specify the dispatch queue on which to call the controls delegate methods.

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

func setControlsDelegate((any AVCaptureSessionControlsDelegate)?, queue: dispatch_queue_t?)

Sets a delegate object for the system to call when it activates and presents controls.

protocol AVCaptureSessionControlsDelegate

A protocol that defines the interface to respond to capture control activation and presentation events.

var controlsDelegate: (any AVCaptureSessionControlsDelegate)?

A delegate object that observes changes to the state of capture controls.

