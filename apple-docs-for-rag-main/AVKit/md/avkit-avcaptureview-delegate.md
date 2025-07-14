

- AVKit
- AVCaptureView
-  delegate 

Instance Property

# delegate

The capture view’s delegate object.

macOS 10.10+

``` source
@MainActor
weak var delegate: (any AVCaptureViewDelegate)? { get set }
```

## Discussion

The capture view disables the start recording button if you don’t provide a delegate object.

## See Also

### Configuring the Delegate

protocol AVCaptureViewDelegate

The protocol that defines the methods you can implement to respond to capture view events.

