

- AVFoundation
- AVCaptionRenderer
- AVCaptionRenderer.Scene
-  timeRange 

Instance Property

# timeRange

The time range during which the system doesn’t modify the scene.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var timeRange: CMTimeRange { get }
```

## See Also

### Inspecting the Scene

var hasActiveCaptions: Bool

A Boolean value that indicates whether the scene contains one or more active captions.

var needsPeriodicRefresh: Bool

A Boolean value that indicates whether the scene requires redrawing while your app progresses through the content.

