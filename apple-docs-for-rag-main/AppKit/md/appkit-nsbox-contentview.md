

- AppKit
- NSBox
-  contentView 

Instance Property

# contentView

The receiver’s content view.

macOS

``` source
@MainActor
var contentView: NSView? { get set }
```

## Discussion

The content view of the `NSBox` object. The content view is created automatically when the box is created and resized as the box is resized (you should never send frame-altering messages directly to a box’s content view). You can replace it with an `NSView` of your own.

## See Also

### Managing Content

var contentViewMargins: NSSize

The distances between the border and the content view.

