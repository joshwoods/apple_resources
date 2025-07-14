

- VisionKit
- ImageAnalysisOverlayView
-  init(frame:) 

Initializer

# init(frame:)

Creates an overlay view with the specified frame rectangle.

macOS 13.0+

``` source
@MainActor
override dynamic init(frame frameRect: NSRect)
```

## Parameters 

`frameRect`  

The frame rectangle for view.

## See Also

### Creating overlay views

convenience init(any ImageAnalysisOverlayViewDelegate)

Creates an overlay view with the specified delegate object.

init?(coder: NSCoder)

Creates an overlay view from data in a coder object.

