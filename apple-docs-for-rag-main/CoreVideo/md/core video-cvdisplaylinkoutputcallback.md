

- Core Video
-  CVDisplayLinkOutputCallback 

Type Alias

# CVDisplayLinkOutputCallback

A type for a display link callback function that the system invokes when it’s time for the app to output a video frame.

Mac Catalyst 13.0+macOS 10.4+

``` source
typealias CVDisplayLinkOutputCallback = (CVDisplayLink, UnsafePointer, UnsafePointer, CVOptionFlags, UnsafeMutablePointer, UnsafeMutableRawPointer?) -> CVReturn
```

## Parameters 

`displayLink`  

A display link that requests a frame.

`inNow`  

A pointer to the current time.

`inOutputTime`  

A pointer to the display time for a frame.

`flagsIn`  

Currently unused. Pass 0.

`flagsOut`  

Currently unused. Pass 0.

`displayLinkContext`  

A pointer to app-defined data.

## Discussion

Your app must register a callback function for the system to invoke with the data necessary to process and output a frame of video. Your callback must retrieve the frame with the timestamp that the `inOutputTime` parameter specifies, manipulate it if you require (for example, apply color correction or map onto a surface), and output it to the display.

## See Also

### Callbacks

typealias CVDisplayLinkOutputHandler

