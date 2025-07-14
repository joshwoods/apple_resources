

- MediaExtension
- MEDecodeFrameOptions
-  doNotOutputFrame 

Instance Property

# doNotOutputFrame

A Boolean value that hints to the decoder whether or not it should emit an image buffer for the frame.

macOS 14.0+

``` source
var doNotOutputFrame: Bool { get set }
```

## Discussion

If true, the decoder emits nil instead of a CVImageBuffer instance.

## See Also

### Inspecting frame decoding options

var realTimePlayback: Bool

A Boolean value that hints to the decoder to use a low-power mode that can’t decode faster than 1x real-time.

