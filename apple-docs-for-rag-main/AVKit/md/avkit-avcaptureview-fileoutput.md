

- AVKit
- AVCaptureView
-  fileOutput 

Instance Property

# fileOutput

The capture file output used to record media data.

macOS 10.10+

``` source
@MainActor
var fileOutput: AVCaptureFileOutput? { get }
```

## Discussion

The value of this property is the first capture file output object contained in the session’s outputs array, or `nil` if it has no outputs. In the latter case, the capture view disables the start recording button. However, it may still enable the controls for choosing input sources.

