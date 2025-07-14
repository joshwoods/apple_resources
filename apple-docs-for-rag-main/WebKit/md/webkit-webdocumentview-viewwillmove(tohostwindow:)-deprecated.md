

- WebKit
- WebDocumentView
-  viewWillMove(toHostWindow:) Deprecated

Instance Method

# viewWillMove(toHostWindow:)

Invoked when a web view’s host window is about to change.

macOS 10.3–10.14Deprecated

``` source
func viewWillMove(toHostWindow hostWindow: NSWindow!)
```

**Required**

## Parameters 

`hostWindow`  

The new host window for the view.

## See Also

### Related Documentation

var hostWindow: NSWindow!

The receiver’s host window.

Deprecated

### Attaching to a window

func viewDidMoveToHostWindow()

Invoked when a web view’s host window is set.

**Required**

Deprecated

