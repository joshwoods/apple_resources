

- Video Toolbox
- VTDecodeInfoFlags
-  frameDropped 

Type Property

# frameDropped

A flag that indicates the decode operation dropped a frame.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
static var frameDropped: VTDecodeInfoFlags { get }
```

## See Also

### Flag values

static var asynchronous: VTDecodeInfoFlags

A flag that indicates the decode operation ran asynchronously.

static var skippedLeadingFrameDropped: VTDecodeInfoFlags

A flag that indicates whether the decode process skips leading frames after dropping a synchronization frame.

static var imageBufferModifiable: VTDecodeInfoFlags

A flag that indicates the image buffer is safe to modify.

