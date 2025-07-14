

- AVFoundation
- AVCaptionRenderer
- AVCaptionRenderer.Scene
-  hasActiveCaptions 

Instance Property

# hasActiveCaptions

A Boolean value that indicates whether the scene contains one or more active captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var hasActiveCaptions: Bool { get }
```

## Discussion

Knowing when the renderer has active captions can be useful to scrub to times where captions are present, or skip scenes where no captions exist.

Important

Don’t use this property value to restrict drawing. Instead, draw an empty fill in render(in:for:) when there aren’t active captions to render.

## See Also

### Inspecting the Scene

var timeRange: CMTimeRange

The time range during which the system doesn’t modify the scene.

var needsPeriodicRefresh: Bool

A Boolean value that indicates whether the scene requires redrawing while your app progresses through the content.

