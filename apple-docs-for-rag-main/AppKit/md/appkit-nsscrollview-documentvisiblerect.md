

- AppKit
- NSScrollView
-  documentVisibleRect 

Instance Property

# documentVisibleRect

The portion of the document view, in its own coordinate system, visible through the scroll view’s content view.

macOS

``` source
@MainActor
var documentVisibleRect: NSRect { get }
```

## See Also

### Related Documentation

var documentVisibleRect: NSRect

The exposed rectangle of the clip view’s document view, in the document view’s own coordinate system.

var visibleRect: NSRect

The portion of the view that isn’t clipped by its superviews.

### Determining Component Sizes

var contentSize: NSSize

The size of the scroll view’s content view.

