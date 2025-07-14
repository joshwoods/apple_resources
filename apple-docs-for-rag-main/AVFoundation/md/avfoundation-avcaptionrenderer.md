

- AVFoundation
-  AVCaptionRenderer 

Class

# AVCaptionRenderer

An object that renders captions for display at a particular time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionRenderer
```

## Overview

This object renders a caption scene for a given time from a collection of captions. If there aren’t any captions to display at the specified time, the renderer draws an empty flood fill with a zero alpha or a color.

## Topics

### Configuring the Renderer

var captions: [AVCaption]

The captions to render.

var bounds: CGRect

The drawing bounds of caption scenes.

### Determining Scene Changes

func captionSceneChanges(in: CMTimeRange) -> [AVCaptionRenderer.Scene]

Determine render time ranges within an enclosing time range to account for visual changes among captions.

class Scene

An object that holds a time range and an associated state which indicates when the renderer draws output.

### Rendering a Caption

func render(in: CGContext, for: CMTime)

Draw the captions for the time you specify.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

