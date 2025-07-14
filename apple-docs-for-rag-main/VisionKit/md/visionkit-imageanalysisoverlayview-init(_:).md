

- VisionKit
- ImageAnalysisOverlayView
-  init(\_:) 

Initializer

# init(\_:)

Creates an overlay view with the specified delegate object.

macOS 13.0+

``` source
@MainActor
convenience init(_ delegate: any ImageAnalysisOverlayViewDelegate)
```

## Parameters 

`delegate`  

The object that provides details about the interface.

## See Also

### Creating overlay views

init(frame: NSRect)

Creates an overlay view with the specified frame rectangle.

init?(coder: NSCoder)

Creates an overlay view from data in a coder object.

