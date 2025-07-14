

- AppKit
- NSWindowDelegate
-  window(\_:shouldDragDocumentWith:from:with:) 

Instance Method

# window(\_:shouldDragDocumentWith:from:with:)

Asks the delegate whether a user can drag the document icon from the window’s title bar.

macOS 10.5+

``` source
@MainActor
optional func window(
    _ window: NSWindow,
    shouldDragDocumentWith event: NSEvent,
    from dragImageLocation: NSPoint,
    with pasteboard: NSPasteboard
) -> Bool
```

## Parameters 

`window`  

The window containing the document icon the user wants to drag.

`event`  

The left-mouse down event that triggered the dragging operation.

`dragImageLocation`  

The location of the origin of the document icon, in window coordinates, when the user started the dragging operation.

`pasteboard`  

The pasteboard containing the contents of the document, which the delegate can modify.

## Return Value

true to allow the drag to proceed; false to prevent it. Before turning no the delegate can implement its own dragging behavior as described below.

## Discussion

Implementing this method enables an application to customize the process of dragging the window’s document icon. The delegate can prohibit the drag by returning false. Before returning false, the delegate can implement its own dragging behavior using drag(_:at:offset:event:pasteboard:source:slideBack:).

Alternatively, the delegate can enable a drag by returning true, for example, to override the default `NSWindow` behavior of prohibiting the drag of an edited document. In addition, the delegate can customize the pasteboard contents before returning true.

## See Also

### Related Documentation

var representedURL: URL?

The URL of the file the window represents.

