

- AVFoundation
- AVCaptionRenderer
-  AVCaptionRenderer.Scene 

Class

# AVCaptionRenderer.Scene

An object that holds a time range and an associated state which indicates when the renderer draws output.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class Scene
```

## Overview

To render a scene, the object considers state like the existence of captions and regions, their temporal overlaps, and whether captions use animation effects. Your app can request time ranges where visual differences exist and use these time ranges to optimize drawing performance, like drawing once per scene. Alternatively, it can ignore scenes, and instead call render(in:for:) repeatedly, but this may have additional performance impact.

## Topics

### Inspecting the Scene

var timeRange: CMTimeRange

The time range during which the system doesn’t modify the scene.

var hasActiveCaptions: Bool

A Boolean value that indicates whether the scene contains one or more active captions.

var needsPeriodicRefresh: Bool

A Boolean value that indicates whether the scene requires redrawing while your app progresses through the content.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Determining Scene Changes

func captionSceneChanges(in: CMTimeRange) -> [AVCaptionRenderer.Scene]

Determine render time ranges within an enclosing time range to account for visual changes among captions.

