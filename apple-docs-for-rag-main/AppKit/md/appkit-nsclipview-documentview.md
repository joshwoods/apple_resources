

- AppKit
- NSClipView
-  documentView 

Instance Property

# documentView

The clip view’s document view.

macOS

``` source
@MainActor
var documentView: NSView? { get set }
```

## Discussion

If the clip view is contained in an NSScrollView, you should send the NSScrollView a documentView message instead, so it can perform whatever updating it needs. Setting this property to a view removes any previous document view, and sets the origin of the clip view’s bounds rectangle to the origin of the new view’s frame rectangle. Doing so also registers the clip view for the notifications frameDidChangeNotification and boundsDidChangeNotification, adjusts the key view loop to include the new document view, and updates a parent NSScrollView display if needed using reflectScrolledClipView(_:).

## See Also

### Related Documentation

Cocoa Drawing Guide

