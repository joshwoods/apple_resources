

- AVFoundation
- AVCaptureScreenInput
-  capturesCursor 

Instance Property

# capturesCursor

A Boolean value that specifies whether the mouse cursor appears in the captured output.

macOS 10.8+

``` source
var capturesCursor: Bool { get set }
```

## Discussion

When this property is true (the default), captured video frames include the mouse pointer. If you change this property to false, the captured output contains only the windows on the screen (that is, the mouse pointer is invisible in captured video).

Note

Even if you hide the mouse pointer in captured output, CMSampleBuffer objects vended by the capture include metadata for the cursor position and mouse button state. See kCMIOSampleBufferAttachmentKey_MouseAndKeyboardModifiers.

## See Also

### Capturing Mouse Activity

var capturesMouseClicks: Bool

A Boolean value that specifies whether mouse clicks appear highlighted in the captured output.

