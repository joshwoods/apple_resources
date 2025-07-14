

- Video Toolbox
- VTDecodeInfoFlags
-  skippedLeadingFrameDropped 

Type Property

# skippedLeadingFrameDropped

A flag that indicates whether the decode process skips leading frames after dropping a synchronization frame.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
static var skippedLeadingFrameDropped: VTDecodeInfoFlags { get }
```

## Discussion

This condition occurs when you performs a seek to a sync frame, and due to frame reordering, there are leading frames following the sync frame that the system can’t decode due to missing references. Dropping these frames has no impact on playback because the nondecodeable frames won’t render.

If the system sets this flag, it sets the frameDropped flag as well.

## See Also

### Flag values

static var asynchronous: VTDecodeInfoFlags

A flag that indicates the decode operation ran asynchronously.

static var frameDropped: VTDecodeInfoFlags

A flag that indicates the decode operation dropped a frame.

static var imageBufferModifiable: VTDecodeInfoFlags

A flag that indicates the image buffer is safe to modify.

