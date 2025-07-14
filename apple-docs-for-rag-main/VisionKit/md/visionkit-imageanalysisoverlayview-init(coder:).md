

- VisionKit
- ImageAnalysisOverlayView
-  init(coder:) 

Initializer

# init(coder:)

Creates an overlay view from data in a coder object.

macOS 13.0+

``` source
@MainActor
required dynamic init?(coder: NSCoder)
```

## Parameters 

`coder`  

The object that contains the data.

## See Also

### Creating overlay views

convenience init(any ImageAnalysisOverlayViewDelegate)

Creates an overlay view with the specified delegate object.

init(frame: NSRect)

Creates an overlay view with the specified frame rectangle.

