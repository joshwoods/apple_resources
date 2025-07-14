

- AVKit
-  AVCaptureViewDelegate 

Protocol

# AVCaptureViewDelegate

The protocol that defines the methods you can implement to respond to capture view events.

macOS 10.9+

``` source
protocol AVCaptureViewDelegate : NSObjectProtocol
```

## Topics

### Starting a New Recording

func captureView(AVCaptureView, startRecordingTo: AVCaptureFileOutput)

Tells the delegate that the user has made a request to start a new recording.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring the Delegate

var delegate: (any AVCaptureViewDelegate)?

The capture view’s delegate object.

