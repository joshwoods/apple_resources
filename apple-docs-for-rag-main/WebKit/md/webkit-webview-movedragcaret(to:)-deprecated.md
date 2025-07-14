

- WebKit
- WebView
-  moveDragCaret(to:) Deprecated

Instance Method

# moveDragCaret(to:)

Moves the drag caret that indicates the destination of a drag operation to a given point.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func moveDragCaret(to point: NSPoint)
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`point`  

The point to move the drag caret to.

## See Also

### Dragging

func element(at: NSPoint) -> [AnyHashable : Any]!

Returns a dictionary description of the element at a given point in the receiver’s coordinates.

Deprecated

func removeDragCaret()

Removes the drag caret that indicates the destination of a drag operation.

Deprecated

