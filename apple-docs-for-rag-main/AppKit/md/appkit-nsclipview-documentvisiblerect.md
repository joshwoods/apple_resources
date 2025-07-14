

- AppKit
- NSClipView
-  documentVisibleRect 

Instance Property

# documentVisibleRect

The exposed rectangle of the clip view’s document view, in the document view’s own coordinate system.

macOS

``` source
@MainActor
var documentVisibleRect: NSRect { get }
```

## Discussion

Note that this rectangle doesn’t reflect the effects of any clipping that may occur above the NSClipView itself. To get the portion of the document view that’s guaranteed to be visible, send it a `visibleRect` message.

## See Also

### Accessing the Visible Portion

var documentRect: NSRect

The rectangle defining the document view’s frame, adjusted to the size of the clip view if the document view is smaller.

