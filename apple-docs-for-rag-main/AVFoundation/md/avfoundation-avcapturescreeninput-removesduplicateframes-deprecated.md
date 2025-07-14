

- AVFoundation
- AVCaptureScreenInput
-  removesDuplicateFrames Deprecated

Instance Property

# removesDuplicateFrames

A Boolean value that specifies whether the capture input skips duplicate frames.

macOS 10.8–10.10Deprecated

``` source
var removesDuplicateFrames: Bool { get set }
```

Deprecated

The capture system ignores this property in macOS 10.10 and later: the capture input never removes duplicate frames. You can re-create this functionality by using AVCaptureVideoDataOutput and comparing successive frames.

