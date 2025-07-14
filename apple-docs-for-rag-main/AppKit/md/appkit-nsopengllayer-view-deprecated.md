

- AppKit
- NSOpenGLLayer
-  view Deprecated

Instance Property

# view

Returns the view associated with the layer.

macOS 10.6–10.14Deprecated

``` source
weak var view: NSView? { get set }
```

Deprecated

Please use CAMetalLayer instead.

## Discussion

Subclasses shouldn’t invoke setView:, but can override it if desired to intercept the layer’s association to, or dissociation from, a view.

