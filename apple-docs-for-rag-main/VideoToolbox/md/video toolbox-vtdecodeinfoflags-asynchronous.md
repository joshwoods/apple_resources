

- Video Toolbox
- VTDecodeInfoFlags
-  asynchronous 

Type Property

# asynchronous

A flag that indicates the decode operation ran asynchronously.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
static var asynchronous: VTDecodeInfoFlags { get }
```

## See Also

### Flag values

static var frameDropped: VTDecodeInfoFlags

A flag that indicates the decode operation dropped a frame.

static var skippedLeadingFrameDropped: VTDecodeInfoFlags

A flag that indicates whether the decode process skips leading frames after dropping a synchronization frame.

static var imageBufferModifiable: VTDecodeInfoFlags

A flag that indicates the image buffer is safe to modify.

