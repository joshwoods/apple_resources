

- AppKit
- NSView
-  globalFrameDidChangeNotification Deprecated

Type Property

# globalFrameDidChangeNotification

Posted whenever an `NSView` object that has attached surfaces (that is, `NSOpenGLContext` objects) moves to a different screen, or other cases where the `NSOpenGLContext` object needs to be updated.

macOS 10.0–10.14Deprecated

``` source
class let globalFrameDidChangeNotification: NSNotification.Name
```

Deprecated

Use NSOpenGLView instead.

## Discussion

The notification object is the surface’s view. This notification does not contain a `userInfo` dictionary.

