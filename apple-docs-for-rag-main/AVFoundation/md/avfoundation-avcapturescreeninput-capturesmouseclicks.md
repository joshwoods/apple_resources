

- AVFoundation
- AVCaptureScreenInput
-  capturesMouseClicks 

Instance Property

# capturesMouseClicks

A Boolean value that specifies whether mouse clicks appear highlighted in the captured output.

macOS 10.7+

``` source
var capturesMouseClicks: Bool { get set }
```

## Discussion

By default, `AVCaptureScreenInput` does not highlight mouse clicks in its captured output.

If you set this property is set to true, mouse clicks are highlighted (a circle is drawn around the mouse for the duration of the click) in the captured output.

## See Also

### Capturing Mouse Activity

var capturesCursor: Bool

A Boolean value that specifies whether the mouse cursor appears in the captured output.

