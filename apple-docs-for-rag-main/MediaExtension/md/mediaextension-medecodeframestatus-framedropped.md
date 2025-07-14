

- MediaExtension
- MEDecodeFrameStatus
-  frameDropped 

Type Property

# frameDropped

A frame decode operation status that indicates the system dropped the output of the frame for a reason other than an error.

macOS 14.0+

``` source
static var frameDropped: MEDecodeFrameStatus { get }
```

## Discussion

The decoder sets this value if doNotOutputFrame is true.

