

- AppKit
- NSOpenGLView
-  update() Deprecated

Instance Method

# update()

Called by Cocoa when the view’s window moves or when the view itself moves or is resized.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func update()
```

Deprecated

Please use MTKView instead.

## Discussion

The default implementation simply calls the update() method of NSOpenGLContext. You can override this method to perform additional update operations on the context or if you need to add locks for multithreaded access to multiple contexts.

## See Also

### Managing the Visible Region

func reshape()

Called by Cocoa when the view’s visible rectangle or bounds change.

Deprecated

