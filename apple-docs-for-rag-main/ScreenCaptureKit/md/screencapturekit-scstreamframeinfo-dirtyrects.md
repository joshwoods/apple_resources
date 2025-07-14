

- ScreenCaptureKit
- SCStreamFrameInfo
-  dirtyRects 

Type Property

# dirtyRects

A key to retrieve the areas of a video frame that contain changes.

Mac Catalyst 18.2+macOS 12.3+

``` source
static let dirtyRects: SCStreamFrameInfo
```

## Discussion

The associated value is an array of rectangles that represents a union of the rectangles redrawn and moved.

## See Also

### Frame information constants

static let status: SCStreamFrameInfo

A key to retrieve the status of a video frame.

static let displayTime: SCStreamFrameInfo

A key to retrieve the display time of a video frame.

static let scaleFactor: SCStreamFrameInfo

A key to retrieve the scale factor of a video frame.

static let contentScale: SCStreamFrameInfo

A key to retrieve the content scale of a video frame.

static let contentRect: SCStreamFrameInfo

A key to retrieve the content rectangle of a video frame.

static let boundingRect: SCStreamFrameInfo

A key to retrieve the bounding rectangle for a video frame.

static let screenRect: SCStreamFrameInfo

A key to retrieve the onscreen location of captured content.

static let presenterOverlayContentRect: SCStreamFrameInfo

