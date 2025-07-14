

- AppKit
- NSOpenGLView
-  reshape() Deprecated

Instance Method

# reshape()

Called by Cocoa when the view’s visible rectangle or bounds change.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func reshape()
```

Deprecated

Please use MTKView instead.

## Discussion

Cocoa typically calls this method during scrolling and resize operations but may call it in other situations when the view’s rectangles change. The default implementation does nothing. You can override this method if you need to adjust the viewport and display frustum.

## See Also

### Managing the Visible Region

func update()

Called by Cocoa when the view’s window moves or when the view itself moves or is resized.

Deprecated

