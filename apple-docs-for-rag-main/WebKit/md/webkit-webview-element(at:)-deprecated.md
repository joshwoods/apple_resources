

- WebKit
- WebView
-  element(at:) Deprecated

Instance Method

# element(at:)

Returns a dictionary description of the element at a given point in the receiver’s coordinates.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func element(at point: NSPoint) -> [AnyHashable : Any]!
```

Deprecated

No longer supported; please adopt WKWebView.

## Parameters 

`point`  

The point to represent as a dictionary.

## Return Value

A dictionary description of the element at `point` in the receiver’s coordinates.

## See Also

### Dragging

func moveDragCaret(to: NSPoint)

Moves the drag caret that indicates the destination of a drag operation to a given point.

Deprecated

func removeDragCaret()

Removes the drag caret that indicates the destination of a drag operation.

Deprecated

