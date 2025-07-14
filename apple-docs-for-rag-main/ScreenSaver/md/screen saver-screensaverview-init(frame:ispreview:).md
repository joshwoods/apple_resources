

- Screen Saver
- ScreenSaverView
-  init(frame:isPreview:) 

Initializer

# init(frame:isPreview:)

Creates a newly allocated screen saver view with the specified frame rectangle and preview information.

macOS 10.0+

``` source
@MainActor
init?(
    frame: NSRect,
    isPreview: Bool
)
```

## Parameters 

`frame`  

The frame rectangle for the view.

`isPreview`  

true if this view provides a preview for system settings, or false if the system fills the screen with your view’s contents.

## Discussion

The screen saver application installs the new view object into the view hierarchy of an NSWindow before the animation begins. This method is the designated initializer for the ScreenSaverView class. Returns `self`.

