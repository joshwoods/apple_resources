

- AppKit
- NSClipView
-  documentCursor 

Instance Property

# documentCursor

The cursor object used when the pointer lies over the view.

macOS

``` source
@MainActor
var documentCursor: NSCursor? { get set }
```

## Discussion

The default value of this property is `nil`, unless you specify a value in the xib file associated with the clip view (or scroll view). Note that the clip view’s document view may specify a cursor for its enclosing scroll view by setting enclosingScrollView.

